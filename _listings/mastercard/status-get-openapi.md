---
swagger: "2.0"
x-collection-name: MasterCard
x-complete: 0
info:
  title: Mastercard Get Status
  description: |-
    Gets general metadata about the current state of the blockchain network.
    Useful for building dashboards.
  version: 1.0.0
host: eas5stl0.mastercard.int:13046
basePath: /z0/core/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /status:
    get:
      summary: Get Status
      description: |-
        Gets general metadata about the current state of the blockchain network.
        Useful for building dashboards.
      operationId: getStatus
      x-api-path-slug: status-get
      parameters:
      - in: header
        name: MCWSSAML
        description: SAML Authorization
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Status
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