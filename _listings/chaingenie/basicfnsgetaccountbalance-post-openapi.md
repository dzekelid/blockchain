---
swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 0
info:
  title: ChainGenie Get user's account balance (*)
  description: Get information about an user's account balance.  The call is restricted
    to the unlocked user's account / query only. <br/>* In this sandbox, you can query
    any user's account balance for testing purposes.  All accounts are test accounts
    and no actual value or account is exposed in the sandbox.
  version: "1.0"
host: api.chaingenie.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ethledger/ipfsget:
    post:
      summary: Retrieve document from IPFS
      description: Retrieve the document stream from IPFS node
      operationId: EthledgerIpfsgetPost
      x-api-path-slug: ethledgeripfsget-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: hash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Retrieve
      - Document
      - From
      - IPFS
  /ethledger/ipfsadd:
    post:
      summary: Write document to IPFS
      description: Post the document into ipfs for safekeep!
      operationId: EthledgerIpfsaddPost
      x-api-path-slug: ethledgeripfsadd-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: files
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Write
      - Document
      - To
      - IPFS
  /basicfns/GetAccountBalance:
    post:
      summary: Get user's account balance (*)
      description: Get information about an user's account balance.  The call is restricted
        to the unlocked user's account / query only. <br/>* In this sandbox, you can
        query any user's account balance for testing purposes.  All accounts are test
        accounts and no actual value or account is exposed in the sandbox.
      operationId: BasicfnsGetAccountBalancePost
      x-api-path-slug: basicfnsgetaccountbalance-post
      parameters:
      - in: formData
        name: accountId
      - in: header
        name: ApiKey
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Users
      - Account
      - Balance
      - (*)
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