---
swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 0
info:
  title: ChainGenie Write document to IPFS
  description: Post the document into ipfs for safekeep!
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