---
swagger: "2.0"
x-collection-name: Lisk
x-complete: 0
info:
  title: Lisk Requests voters data for a delegate
  description: |-
    *Attention: At least **one of the filter parameters must be provided.***
    Returns all votes received by a delegate.
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
  /signatures:
    post:
      summary: Submits a signature object to sign multisignature transactions
      description: |-
        Submits signature to sign a multisignature transaction.
        Signature objects can be generated locally either by using Lisk Commander or with Lisk Elements.
      operationId: postSignature
      x-api-path-slug: signatures-post
      parameters:
      - in: body
        name: signature
        description: Signature object to submit to the network
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Submits
      - Signature
      - Object
      - To
      - Sign
      - Multisignature
      - Transactions
  /votes:
    get:
      summary: Requests votes data for an account
      description: |-
        *Attention: At least **one of the filter parameters must be provided.***
        Returns all votes placed by an account.
      operationId: getVotes
      x-api-path-slug: votes-get
      parameters:
      - in: query
        name: address
        description: Address of an account
      - in: query
        name: limit
        description: Limit applied to results
      - in: query
        name: offset
        description: Offset value for results
      - in: query
        name: publicKey
        description: Public key to query
      - in: query
        name: secondPublicKey
        description: Second public key to query
      - in: query
        name: sort
        description: Fields to sort results by
      - in: query
        name: username
        description: Delegate username to query
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Votes
      - Dataan
      - Account
  /voters:
    get:
      summary: Requests voters data for a delegate
      description: |-
        *Attention: At least **one of the filter parameters must be provided.***
        Returns all votes received by a delegate.
      operationId: getVoters
      x-api-path-slug: voters-get
      parameters:
      - in: query
        name: address
        description: Address of an account
      - in: query
        name: limit
        description: Limit applied to results
      - in: query
        name: offset
        description: Offset value for results
      - in: query
        name: publicKey
        description: Public key to query
      - in: query
        name: secondPublicKey
        description: Second public key to query
      - in: query
        name: sort
        description: Fields to sort results by
      - in: query
        name: username
        description: Delegate username to query
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Voters
      - Dataa
      - Delegate
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