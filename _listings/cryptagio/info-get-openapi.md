---
swagger: "2.0"
x-collection-name: Cryptagio
x-complete: 0
info:
  title: Cryptagio Get Info
  description: Get information..
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /info:
    get:
      summary: Get Info
      description: Get information..
      operationId: getInfo
      x-api-path-slug: info-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Info
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