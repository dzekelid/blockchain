---
swagger: "2.0"
x-collection-name: Blockchain
x-complete: 0
info:
  title: Blockchain Info Stats
  description: This method can be used to get the data behind Blockchain.info's stats.
  version: 1.0.0
host: blockchain.info
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ticker:
    get:
      summary: Ticker
      description: Returns a JSON object with the currency codes as keys. "15m" is
        the 15 minutes delayed market price, "last" is the most recent market price,
        "symbol" is the currency symbol.
      operationId: getTicker
      x-api-path-slug: ticker-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Ticker
  /tobtc:
    get:
      summary: Convert
      description: Convert x value in the provided currency to btc.
      operationId: convertToBTC
      x-api-path-slug: tobtc-get
      parameters:
      - in: query
        name: currency
        description: A currency code
        type: string
        format: string
      - in: query
        name: value
        description: Value to convert
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Conversion
  /stats:
    get:
      summary: Stats
      description: This method can be used to get the data behind Blockchain.info's
        stats.
      operationId: getStats
      x-api-path-slug: stats-get
      parameters:
      - in: query
        name: format
        description: The format to return (json,html)
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Statistics
x-streamrank:
  polling_total_time_average: "0.17"
  polling_size_download_average: "705.04"
  streaming_total_time_average: "0.11"
  streaming_size_download_average: "359.88"
  change_yes: "158"
  change_no: "1315"
  time_percentage: "38"
  size_percentage: "49"
  change_percentage: "11"
  last_run: "2018-02-21"
  days_run: "1"
  minute_run: "0"
---