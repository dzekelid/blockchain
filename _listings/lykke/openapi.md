swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
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