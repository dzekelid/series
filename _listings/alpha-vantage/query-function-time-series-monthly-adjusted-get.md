---
swagger: "2.0"
info:
  title: Alpha Vantage Monthly Time Series Adjusted
  description: This API returns monthly adjusted time series (last trading day of
    each month, monthly open, monthly high, monthly low, monthly close, monthly adjusted
    close, monthly volume, monthly dividend) of the equity specified, covering up
    to 20 years of historical data.
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
  /query?function=TIME_SERIES_MONTHLY_ADJUSTED:
    get:
      summary: Monthly Time Series Adjusted
      description: This API returns monthly adjusted time series (last trading day
        of each month, monthly open, monthly high, monthly low, monthly close, monthly
        adjusted close, monthly volume, monthly dividend) of the equity specified,
        covering up to 20 years of historical data
      operationId: getMonthlyTimeSeriesAdjusted
      parameters:
      - in: query
        name: symbol
        description: The stocker ticker symbol
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - market data
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