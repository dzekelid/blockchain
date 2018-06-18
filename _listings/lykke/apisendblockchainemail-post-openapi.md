---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Add API Sendblockchainemail
  version: 1.0.0
  description: Add api sendblockchainemail.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/BlockchainTransaction:
    get:
      summary: Get API Blockchaintransaction
      description: Get api blockchaintransaction.
      operationId: ApiBlockchainTransactionGet
      x-api-path-slug: apiblockchaintransaction-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: blockChainHash
      responses:
        200:
          description: OK
      tags:
      - Blockchaintransaction
  /api/SendBlockchainEmail:
    post:
      summary: Add API Sendblockchainemail
      description: Add api sendblockchainemail.
      operationId: ApiSendBlockchainEmailPost
      x-api-path-slug: apisendblockchainemail-post
      parameters:
      - in: query
        name: assetId
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Sendblockchainemail
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