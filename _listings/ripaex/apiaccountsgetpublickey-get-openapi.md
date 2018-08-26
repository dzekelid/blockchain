---
swagger: "2.0"
x-collection-name: RipaEx
x-complete: 0
info:
  title: RipaEx Accounts Get Publickey
  description: Get the public key of an account.
  version: 1.0.0
host: api.ripaex.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/accounts/getBalance:
    get:
      summary: Accounts Get Balance
      description: Get the balance of an account.
      operationId: accounts.getBalance
      x-api-path-slug: apiaccountsgetbalance-get
      parameters:
      - in: query
        name: address
        description: A valid RIPA Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Accounts
      - ""
      - Balance
  /api/accounts/getPublickey:
    get:
      summary: Accounts Get Publickey
      description: Get the public key of an account.
      operationId: accounts.getPublickey
      x-api-path-slug: apiaccountsgetpublickey-get
      parameters:
      - in: query
        name: address
        description: A valid RIPA Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Accounts
      - ""
      - Publickey
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