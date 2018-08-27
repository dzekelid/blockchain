---
swagger: "2.0"
x-collection-name: Lisk
x-complete: 0
info:
  title: Lisk Requests transactions data
  description: Search for a specified transaction in the system.
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
    get:
      summary: Requests transactions data
      description: Search for a specified transaction in the system.
      operationId: getTransactions
      x-api-path-slug: transactions-get
      parameters:
      - in: query
        name: blockId
        description: Block id to query
      - in: query
        name: fromTimestamp
        description: Starting unix timestamp
      - in: query
        name: height
        description: Current height of the network
      - in: query
        name: id
        description: Transaction id to query
      - in: query
        name: limit
        description: Limit applied to results
      - in: query
        name: maxAmount
        description: Maximum transaction amount in Beddows
      - in: query
        name: minAmount
        description: Minimum transaction amount in Beddows
      - in: query
        name: offset
        description: Offset value for results
      - in: query
        name: recipientId
        description: Recipient lisk address
      - in: query
        name: recipientPublicKey
        description: Recipient public key
      - in: query
        name: senderId
        description: Sender lisk address
      - in: query
        name: senderIdOrRecipientId
        description: Lisk address
      - in: query
        name: senderPublicKey
        description: Sender public key
      - in: query
        name: sort
        description: Fields to sort results by
      - in: query
        name: toTimestamp
        description: Ending unix timestamp
      - in: query
        name: type
        description: Transaction type (0-7)
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Transactions
      - Data
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