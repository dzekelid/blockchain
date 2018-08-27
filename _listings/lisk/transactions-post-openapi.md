---
swagger: "2.0"
x-collection-name: Lisk
x-complete: 0
info:
  title: Lisk Submits signed transaction for processing
  description: |-
    Submits signed transaction object for processing by the transaction pool.
    Transaction objects can be generated locally either by using Lisk Commander or with Lisk Elements.
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /spec:
    x-swagger-pipe:
      summary: ""
      description: ""
      operationId: ""
      x-api-path-slug: spec-xswaggerpipe
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - ""
  /transactions:
    post:
      summary: Submits signed transaction for processing
      description: |-
        Submits signed transaction object for processing by the transaction pool.
        Transaction objects can be generated locally either by using Lisk Commander or with Lisk Elements.
      operationId: postTransaction
      x-api-path-slug: transactions-post
      parameters:
      - in: body
        name: transaction
        description: Transaction object to submit to the network
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Submits
      - Signed
      - Transactionprocessing
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