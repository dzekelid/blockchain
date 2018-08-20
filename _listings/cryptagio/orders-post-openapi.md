---
swagger: "2.0"
x-collection-name: Cryptagio
x-complete: 0
info:
  title: Cryptagio Post Orders
  description: Accepts an array of JSON objects.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /info:
    get:
      summary: Get Info
      description: Get information..
      operationId: getInfo
      x-api-path-slug: info-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Info
  /ticker:
    get:
      summary: Get Ticker
      description: Get ticker of all markets..
      operationId: getTicker
      x-api-path-slug: ticker-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Ticker
  /trades:
    get:
      summary: Get Trades
      description: Get recent trades on market, each trade is included only once.
        Trades are sorted in reverse creation order.
      operationId: getTrades
      x-api-path-slug: trades-get
      parameters:
      - in: query
        name: from_time
        description: Filter trades by time
      - in: query
        name: from_uuid
        description: Filter trades by id
      - in: query
        name: limit
        description: Limit the number of returned trades
      - in: query
        name: market
        description: Filter trades by market
      - in: query
        name: order
        description: If set, returned orders will be sorted in specific order
      - in: query
        name: side
      - in: query
        name: to_time
        description: Filter trades by time
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Trades
  /trades/my:
    get:
      summary: Get My Trades
      description: Trades are sorted in reverse creation order.
      operationId: getTradesMy
      x-api-path-slug: tradesmy-get
      parameters:
      - in: query
        name: from_time
        description: Filter trades by time
      - in: query
        name: from_uuid
        description: Filter trades by id
      - in: query
        name: limit
        description: Limit the number of returned trades
      - in: query
        name: market
        description: Filter trades by market
      - in: query
        name: order
        description: If set, returned orders will be sorted in specific order
      - in: query
        name: side
      - in: query
        name: to_time
        description: Filter trades by time
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Trades
      - My
  /balances:
    get:
      summary: Get Balances
      description: Get user balances..
      operationId: getBalances
      x-api-path-slug: balances-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Balances
  /orders/my:
    get:
      summary: GetMy  Orders
      description: Trades are sorted in reverse creation order.
      operationId: getOrdersMy
      x-api-path-slug: ordersmy-get
      parameters:
      - in: query
        name: from_time
        description: Filter trades by time
      - in: query
        name: from_uuid
        description: Filter orders by id
      - in: query
        name: limit
        description: Limit the number of returned trades
      - in: query
        name: market
        description: Filter orders by market
      - in: query
        name: order
        description: If set, returned orders will be sorted in specific order
      - in: query
        name: side
        description: Filter orders by side
      - in: query
        name: status
        description: Filter orders by status
      - in: query
        name: to_time
        description: Filter trades by time
      - in: query
        name: type
        description: Filter orders by type
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Orders
      - My
  /orders:
    post:
      summary: Post Orders
      description: Accepts an array of JSON objects.
      operationId: postOrders
      x-api-path-slug: orders-post
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Orders
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