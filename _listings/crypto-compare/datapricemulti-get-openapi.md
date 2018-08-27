---
swagger: "2.0"
x-collection-name: Crypto Compare
x-complete: 0
info:
  title: Crypto Compare Get Multiple Prices
  description: Get multiple prices.
  version: 1.0.0
host: min-api.cryptocompare.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /data/price:
    get:
      summary: Get Single Price
      description: Get single price.
      operationId: DataPriceGet
      x-api-path-slug: dataprice-get
      parameters:
      - in: query
        name: fsym
      - in: query
        name: tsyms
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Single
      - Price
  /data/pricemulti:
    get:
      summary: Get Multiple Prices
      description: Get multiple prices.
      operationId: DataPricemultiGet
      x-api-path-slug: datapricemulti-get
      parameters:
      - in: query
        name: fsyms
      - in: query
        name: tsyms
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Multiple
      - Prices
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