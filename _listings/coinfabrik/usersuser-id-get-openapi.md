---
swagger: "2.0"
x-collection-name: CoinFabrik
x-complete: 0
info:
  title: CoinFabrik Show a user
  description: "Get any user\u2019s public information with their ID."
  contact:
    name: CoinFabrik
    url: http://www.coinfabrik.com/
  version: 1.0.0
host: api.coinbase.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{user_id}:
    get:
      summary: Show a user
      description: "Get any user\u2019s public information with their ID."
      operationId: get-any-users-public-information-with-their-id
      x-api-path-slug: usersuser-id-get
      parameters:
      - in: path
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Show
      - User
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