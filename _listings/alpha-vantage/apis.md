---
name: Alpha Vantage
x-slug: alpha-vantage
description: Composed of a tight-knit community of researchers, engineers, and business
  professionals, Alpha Vantage Inc. is a leading provider of free APIs for realtime
  and historical data on stocks, physical currencies, and digital/crypto currencies.
  Our success is driven by rigorous research, cutting edge technology, and a disciplined
  focus on democratizing access to data.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
  Shot 2018-01-22 at 4.52.35 PM.png
x-kinRank: "8"
x-alexaRank: "160846"
tags: Series
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/alpha-vantage/apis.md
specificationVersion: "0.14"
apis:
- name: Alpha Vantage Intraday Time Series
  x-api-slug: alpha-vantage
  description: This API returns intraday time series (timestamp, open, high, low,
    close, volume) of the equity specified, updated realtime.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2018-01-22 at 4.52.35 PM.png
  humanURL: https://www.alphavantage.co
  baseURL: https://www.alphavantage.co////query?function=TIME_SERIES_INTRADAY
  tags: Market Data, Time Series
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/alpha-vantage/queryfunctiontime-series-intraday-get-openapi.md
- name: Alpha Vantage Daily Time Series Adjusted
  x-api-slug: alpha-vantage
  description: This API returns daily time series (date, daily open, daily high, daily
    low, daily close, daily volume, daily adjusted close, and split/dividend events)
    of the equity specified, covering up to 20 years of historical data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2018-01-22 at 4.52.35 PM.png
  humanURL: https://www.alphavantage.co
  baseURL: https://www.alphavantage.co////query?function=TIME_SERIES_DAILY_ADJUSTED
  tags: Market Data, Time Series
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/alpha-vantage/queryfunctiontime-series-daily-adjusted-get-openapi.md
- name: Alpha Vantage Weekly Time Series
  x-api-slug: alpha-vantage
  description: This API returns weekly time series (last trading day of each week,
    weekly open, weekly high, weekly low, weekly close, weekly volume) of the equity
    specified, covering up to 20 years of historical data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2018-01-22 at 4.52.35 PM.png
  humanURL: https://www.alphavantage.co
  baseURL: https://www.alphavantage.co////query?function=TIME_SERIES_WEEKLY
  tags: Market Data, Time Series
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/alpha-vantage/queryfunctiontime-series-weekly-get-openapi.md
- name: Alpha Vantage Daily Time Series
  x-api-slug: alpha-vantage
  description: This API returns daily time series (date, daily open, daily high, daily
    low, daily close, daily volume) of the equity specified, covering up to 20 years
    of historical data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2018-01-22 at 4.52.35 PM.png
  humanURL: https://www.alphavantage.co
  baseURL: https://www.alphavantage.co////query?function=TIME_SERIES_DAILY
  tags: Market Data, Time Series
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/alpha-vantage/queryfunctiontime-series-daily-get-openapi.md
- name: Alpha Vantage Monthly Time Series
  x-api-slug: alpha-vantage
  description: This API returns monthly time series (last trading day of each month,
    monthly open, monthly high, monthly low, monthly close, monthly volume) of the
    equity specified, covering up to 20 years of historical data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2018-01-22 at 4.52.35 PM.png
  humanURL: https://www.alphavantage.co
  baseURL: https://www.alphavantage.co////query?function=TIME_SERIES_MONTHLY
  tags: Market Data, Time Series
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/alpha-vantage/queryfunctiontime-series-monthly-get-openapi.md
- name: Alpha Vantage Monthly Time Series Adjusted
  x-api-slug: alpha-vantage
  description: This API returns monthly adjusted time series (last trading day of
    each month, monthly open, monthly high, monthly low, monthly close, monthly adjusted
    close, monthly volume, monthly dividend) of the equity specified, covering up
    to 20 years of historical data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2018-01-22 at 4.52.35 PM.png
  humanURL: https://www.alphavantage.co
  baseURL: https://www.alphavantage.co////query?function=TIME_SERIES_MONTHLY_ADJUSTED
  tags: Market Data, Time Series
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/alpha-vantage/queryfunctiontime-series-monthly-adjusted-get-openapi.md
- name: Alpha Vantage Batch Stock Quotes
  x-api-slug: alpha-vantage
  description: The batch stock quotes API enables the querying of multiple stock quotes
    with a single API request, updated realtime. It may serve as a lightweight alternative
    to our core stock time series APIs above (which have richer content but are symbol-specific).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2018-01-22 at 4.52.35 PM.png
  humanURL: https://www.alphavantage.co
  baseURL: https://www.alphavantage.co////query?function=BATCH_STOCK_QUOTES
  tags: Market Data,Time Series, Stock Quotes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/alpha-vantage/queryfunctionbatch-stock-quotes-get-openapi.md
- name: Alpha Vantage Digital Currencies Intraday
  x-api-slug: alpha-vantage
  description: This API returns the realtime intraday time series (in 5-minute intervals)
    for any digital currency (e.g., BTC) traded on a specific market (e.g., CNY/Chinese
    Yuan). Prices and volumes are quoted in both the market-specific currency and
    USD.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2018-01-22 at 4.52.35 PM.png
  humanURL: https://www.alphavantage.co
  baseURL: https://www.alphavantage.co////query?function=DIGITAL_CURRENCY_INTRADAY
  tags: Market Data,Digital Currencies,Intraday,Time Series
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/alpha-vantage/queryfunctiondigital-currency-intraday-get-openapi.md
- name: Alpha Vantage Digital Currencies Daily
  x-api-slug: alpha-vantage
  description: This API returns the daily historical time series for a digital currency
    (e.g., BTC) traded on a specific market (e.g., CNY/Chinese Yuan), refreshed daily
    at midnight (UTC). Prices and volumes are quoted in both the market-specific currency
    and USD.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2018-01-22 at 4.52.35 PM.png
  humanURL: https://www.alphavantage.co
  baseURL: https://www.alphavantage.co////query?function=DIGITAL_CURRENCY_DAILY
  tags: Market Data,Digital Currencies,Daily,Time Series
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/alpha-vantage/queryfunctiondigital-currency-daily-get-openapi.md
- name: Alpha Vantage Digital Currencies Weekly
  x-api-slug: alpha-vantage
  description: This API returns the weekly historical time series for a digital currency
    (e.g., BTC) traded on a specific market (e.g., CNY/Chinese Yuan), refreshed daily
    at midnight (UTC). Prices and volumes are quoted in both the market-specific currency
    and USD.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2018-01-22 at 4.52.35 PM.png
  humanURL: https://www.alphavantage.co
  baseURL: https://www.alphavantage.co////query?function=DIGITAL_CURRENCY_WEEKLY
  tags: Market Data,Digital Currencies,Weekly,Time Series
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/alpha-vantage/queryfunctiondigital-currency-weekly-get-openapi.md
- name: Alpha Vantage Digital Currencies Monthly
  x-api-slug: alpha-vantage
  description: This API returns the monthly historical time series for a digital currency
    (e.g., BTC) traded on a specific market (e.g., CNY/Chinese Yuan), refreshed daily
    at midnight (UTC). Prices and volumes are quoted in both the market-specific currency
    and USD.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2018-01-22 at 4.52.35 PM.png
  humanURL: https://www.alphavantage.co
  baseURL: https://www.alphavantage.co////query?function=DIGITAL_CURRENCY_MONTHLY
  tags: Market Data,Digital Currencies,Monthly,Time Series
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/alpha-vantage/queryfunctiondigital-currency-monthly-get-openapi.md
- name: Alpha Vantage
  x-api-slug: alpha-vantage
  description: Composed of a tight-knit community of researchers, engineers, and business
    professionals, Alpha Vantage Inc. is a leading provider of free APIs for realtime
    and historical data on stocks, physical currencies, and digital/crypto currencies.
    Our success is driven by rigorous research, cutting edge technology, and a disciplined
    focus on democratizing access to data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2018-01-22 at 4.52.35 PM.png
  humanURL: https://www.alphavantage.co
  baseURL: https://www.alphavantage.co//
  tags: Series
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/alpha-vantage/openapi.md
x-common:
- type: x-command-line-interface
  url: https://www.npmjs.com/package/alpha-vantage-cli
- type: x-documentation
  url: https://www.alphavantage.co/documentation/
- type: x-forum
  url: https://www.alpha-vantage.community/
- type: x-selfservice-registration
  url: https://www.alphavantage.co/support/#api-key
- type: x-support
  url: https://www.alphavantage.co/support/#support
- type: x-terms-of-service
  url: https://www.alphavantage.co/terms_of_service/
- type: x-website
  url: https://www.alphavantage.co
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---