---
swagger: "2.0"
x-collection-name: Blockchain
x-complete: 0
info:
  title: Blockchain Info Raw Transaction
  description: Returns a raw trasaction.
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
  /pools:
    get:
      summary: Pools
      description: This method can be used to get the data behind Blockchain.info's
        pools information.
      operationId: getPools
      x-api-path-slug: pools-get
      parameters:
      - in: query
        name: timespan
        description: Duration over which the data is computed, maximum 10 days, default
          is 4 days (ie
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Pools
  /rawblock/{block_hash}:
    get:
      summary: Raw Block
      description: Returns a single raw block.
      operationId: getRawBlock
      x-api-path-slug: rawblockblock-hash-get
      parameters:
      - in: path
        name: block_hash
        description: The block hash
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
  /rawtx/{tx_hash}:
    get:
      summary: Raw Transaction
      description: Returns a raw trasaction.
      operationId: getRawTransaction
      x-api-path-slug: rawtxtx-hash-get
      parameters:
      - in: query
        name: tx_hash
        description: The hash
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Transactions
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