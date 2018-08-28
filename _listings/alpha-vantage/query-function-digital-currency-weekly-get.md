---
swagger: "2.0"
info:
  title: Alpha Vantage Digital Currencies Weekly
  description: This API returns the weekly historical time series for a digital currency
    (e.g., BTC) traded on a specific market (e.g., CNY/Chinese Yuan), refreshed daily
    at midnight (UTC). Prices and volumes are quoted in both the market-specific currency
    and USD.
  version: 1.0.0
host: www.alphavantage.co
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /query?function=DIGITAL_CURRENCY_WEEKLY:
    get:
      summary: Digital Currencies Weekly
      description: This API returns the weekly historical time series for a digital
        currency (e
      operationId: getDigitalCurrenciesWeekly
      parameters:
      - in: query
        name: market
        description: The exchange market of your choice
        type: string
        format: string
      - in: query
        name: symbol
        description: The digital/crypto currency of your choice
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - market data
      - digital currencies
      - weekly
      - time series
definitions: []
x-collection-name: Alpha Vantage
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---