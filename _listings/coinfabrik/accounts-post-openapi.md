---
swagger: "2.0"
x-collection-name: CoinFabrik
x-complete: 0
info:
  title: CoinFabrik Create account
  description: Creates a new account for user.
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
  /user:
    get:
      summary: Show current user
      description: "Get current user\u2019s public information. To get user\u2019s
        email or private information, use permissions wallet:user:email and wallet:user:read."
      operationId: get-current-users-public-information-to-get-users-email-or-private-information-use-permissions-walle
      x-api-path-slug: user-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Show
      - Current
      - User
    put:
      summary: Update current user
      description: Modify current user and their preferences.
      operationId: modify-current-user-and-their-preferences
      x-api-path-slug: user-put
      parameters:
      - in: body
        name: body
        description: Properties to update
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Current
      - User
  /user/auth:
    get:
      summary: Show authorization information
      description: "Get current user\u2019s authorization information including granted
        scopes and send limits when using OAuth2 authentication."
      operationId: get-current-users-authorization-information-including-granted-scopes-and-send-limits-when-using-oaut
      x-api-path-slug: userauth-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Show
      - Authorization
      - Information
  /accounts:
    get:
      summary: List accounts
      description: "Lists current user\u2019s accounts to which the authentication
        method has access to."
      operationId: lists-current-users-accounts-to-which-the-authentication-method-has-access-to
      x-api-path-slug: accounts-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - List
      - Accounts
    post:
      summary: Create account
      description: Creates a new account for user.
      operationId: creates-a-new-account-for-user
      x-api-path-slug: accounts-post
      parameters:
      - in: body
        name: account_properties
        description: Account properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Account
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