---
swagger: "2.0"
x-collection-name: CoinMarketCap
x-complete: 0
info:
  title: CoinMarketCap Get aggregate market metrics (historical)
  description: |-
    Get an interval of aggregate 24 hour volume and market cap data globally based on time and interval parameters.

    **Technical Details**
    A historic quote for every "interval" period between your "time_start" and "time_end" will be returned.
    If a "time_start" is not supplied, the "interval" will be applied in reverse from "time_end".
    If "time_end" is not supplied, it defaults to the current time.
    At each "interval" period, the historic quote that is closest in time to the requested time will be returned.
    If no historic quotes are available in a given "interval" period up until the next interval period, it will be skipped.

    **Interval Options**
    There are 2 types of time interval formats that may be used for "interval".

    The first are calendar year and time constants in UTC time:
    **"hourly"** - Get the first quote available at the beginning of each calendar hour.
    **"daily"** - Get the first quote available at the beginning of each calendar day.
    **"weekly"** - Get the first quote available at the beginning of each calendar week.
    **"monthly"** - Get the first quote available at the beginning of each calendar month.
    **"yearly"** - Get the first quote available at the beginning of each calendar year.

    The second are relative time intervals.
    **"m"**: Get the first quote available every "m" minutes (60 second intervals). Supported minutes are: "5m", "10m", "15m", "30m", "45m".
    **"h"**: Get the first quote available every "h" hours (3600 second intervals). Supported hour intervals are: "1h", "2h", "3h", "6h", "12h".
    **"d"**: Get the first quote available every "d" days (86400 second intervals). Supported day intervals are: "1d", "2d", "3d", "7d", "14d", "15d", "30d", "60d", "90d", "365d".

    **This endpoint is available on the following API plans:**
    - ~~Starter~~
    - ~~Hobbyist~~
    - Standard (1 month)
    - Professional (12 months)
    - Enterprise (Up to 5 years)

    **Cache / Update frequency:** Every ~5 minutes. This endpoint will be migrated to ~1 minute updates shortly.
  termsOfService: https://coinmarketcap.com/terms/
  version: 1.0.0
host: pro-api.coinmarketcap.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/global-metrics/quotes/latest:
    get:
      summary: Get aggregate market metrics (latest)
      description: |-
        Get the latest quote of aggregate market metrics. Use the "convert" option to return market values in multiple fiat and cryptocurrency conversions in the same call.

        **This endpoint is available on the following API plans:**
        - Starter
        - Hobbyist
        - Standard
        - Professional
        - Enterprise

        **Cache / Update frequency:** Every ~5 minutes. This endpoint will be migrated to ~1 minute updates shortly.
      operationId: getV1GlobalmetricsQuotesLatest
      x-api-path-slug: v1globalmetricsquoteslatest-get
      parameters:
      - in: query
        name: convert
        description: Optionally calculate market quotes in up to 32 currencies at
          once by passing a comma-separated list of cryptocurrency or fiat currency
          symbols
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Aggregate
      - Market
      - Metrics
      - (latest)
  /v1/global-metrics/quotes/historical:
    get:
      summary: Get aggregate market metrics (historical)
      description: |-
        Get an interval of aggregate 24 hour volume and market cap data globally based on time and interval parameters.

        **Technical Details**
        A historic quote for every "interval" period between your "time_start" and "time_end" will be returned.
        If a "time_start" is not supplied, the "interval" will be applied in reverse from "time_end".
        If "time_end" is not supplied, it defaults to the current time.
        At each "interval" period, the historic quote that is closest in time to the requested time will be returned.
        If no historic quotes are available in a given "interval" period up until the next interval period, it will be skipped.

        **Interval Options**
        There are 2 types of time interval formats that may be used for "interval".

        The first are calendar year and time constants in UTC time:
        **"hourly"** - Get the first quote available at the beginning of each calendar hour.
        **"daily"** - Get the first quote available at the beginning of each calendar day.
        **"weekly"** - Get the first quote available at the beginning of each calendar week.
        **"monthly"** - Get the first quote available at the beginning of each calendar month.
        **"yearly"** - Get the first quote available at the beginning of each calendar year.

        The second are relative time intervals.
        **"m"**: Get the first quote available every "m" minutes (60 second intervals). Supported minutes are: "5m", "10m", "15m", "30m", "45m".
        **"h"**: Get the first quote available every "h" hours (3600 second intervals). Supported hour intervals are: "1h", "2h", "3h", "6h", "12h".
        **"d"**: Get the first quote available every "d" days (86400 second intervals). Supported day intervals are: "1d", "2d", "3d", "7d", "14d", "15d", "30d", "60d", "90d", "365d".

        **This endpoint is available on the following API plans:**
        - ~~Starter~~
        - ~~Hobbyist~~
        - Standard (1 month)
        - Professional (12 months)
        - Enterprise (Up to 5 years)

        **Cache / Update frequency:** Every ~5 minutes. This endpoint will be migrated to ~1 minute updates shortly.
      operationId: getV1GlobalmetricsQuotesHistorical
      x-api-path-slug: v1globalmetricsquoteshistorical-get
      parameters:
      - in: query
        name: convert
        description: By default market quotes are returned in USD
      - in: query
        name: count
        description: The number of interval periods to return results for
      - in: query
        name: interval
        description: Interval of time to return data points for
      - in: query
        name: time_end
        description: Timestamp (Unix or ISO 8601) to stop returning quotes for (inclusive)
      - in: query
        name: time_start
        description: Timestamp (Unix or ISO 8601) to start returning quotes for
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Aggregate
      - Market
      - Metrics
      - (historical)
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