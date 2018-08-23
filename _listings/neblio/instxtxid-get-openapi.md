---
swagger: "2.0"
x-collection-name: Neblio
x-complete: 0
info:
  title: Neblio Returns transaction object
  description: Returns NEBL transaction object representing a NEBL transaction
  version: 1.0.0
host: ntp1node.nebl.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ntp1/tokenid/{tokensymbol}:
    get:
      summary: Returns the tokenId representing a token
      description: Translates a token symbol to a tokenId if a token exists with that
        symbol on the network
      operationId: getTokenId
      x-api-path-slug: ntp1tokenidtokensymbol-get
      parameters:
      - in: path
        name: tokensymbol
        description: Token symbol
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - TokenId
      - Representing
      - Token
  /ntp1/broadcast:
    post:
      summary: Broadcasts a signed raw transaction to the network
      description: Broadcasts a signed raw transaction to the network. If successful
        returns the txid of the broadcast trasnaction.
      operationId: broadcastTx
      x-api-path-slug: ntp1broadcast-post
      parameters:
      - in: body
        name: body
        description: Object representing a transaction to broadcast
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Broadcasts
      - Signed
      - Raw
      - Transaction
      - To
      - Network
  /ntp1/addressinfo/{address}:
    get:
      summary: Information On a Neblio Address
      description: Returns both NEBL and NTP1 token UTXOs held at the given address.
      operationId: getAddressInfo
      x-api-path-slug: ntp1addressinfoaddress-get
      parameters:
      - in: path
        name: address
        description: Neblio Address to get information on
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Information
      - "On"
      - Neblio
      - Ress
  /ntp1/transactioninfo/{txid}:
    get:
      summary: Information On an NTP1 Transaction
      description: Returns detailed information regarding an NTP1 transaction.
      operationId: getTransactionInfo
      x-api-path-slug: ntp1transactioninfotxid-get
      parameters:
      - in: path
        name: txid
        description: Neblio txid to get information on
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Information
      - "On"
      - NTP1
      - Transaction
  /ntp1/tokenmetadata/{tokenid}:
    get:
      summary: Get Issuance Metadata of Token
      description: Returns the metadata associated with a token at time of issuance.
      operationId: getTokenMetadataOfIssuance
      x-api-path-slug: ntp1tokenmetadatatokenid-get
      parameters:
      - in: path
        name: tokenid
        description: TokenId to request metadata for
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Issuance
      - Metadata
      - Of
      - Token
  /ntp1/tokenmetadata/{tokenid}/{utxo}:
    get:
      summary: Get UTXO Metadata of Token
      description: Returns the metadata associated with a token for that specific
        utxo instead of the issuance transaction.
      operationId: getTokenMetadataOfUtxo
      x-api-path-slug: ntp1tokenmetadatatokenidutxo-get
      parameters:
      - in: path
        name: tokenid
        description: TokenId to request metadata for
      - in: path
        name: utxo
        description: Specific UTXO to request metadata for
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - UTXO
      - Metadata
      - Of
      - Token
  /ntp1/stakeholders/{tokenid}:
    get:
      summary: Get Addresses Holding a Token
      description: Returns the the the addresses holding a token and how many tokens
        are held
      operationId: getTokenHolders
      x-api-path-slug: ntp1stakeholderstokenid-get
      parameters:
      - in: path
        name: tokenid
        description: TokenId to request metadata for
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Resses
      - Holding
      - Token
  /ntp1/issue:
    post:
      summary: Builds a transaction that issues a new NTP1 Token
      description: Builds an unsigned raw transaction that issues a new NTP1 token
        on the Neblio blockchain.
      operationId: issueToken
      x-api-path-slug: ntp1issue-post
      parameters:
      - in: body
        name: body
        description: Object representing the token to be created
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Builds
      - Transaction
      - That
      - Issues
      - New
      - NTP1
      - Token
  /ntp1/sendtoken:
    post:
      summary: Builds a transaction that sends an NTP1 Token
      description: Builds an unsigned raw transaction that sends an NTP1 token on
        the Neblio blockchain.
      operationId: sendToken
      x-api-path-slug: ntp1sendtoken-post
      parameters:
      - in: body
        name: body
        description: Object representing the token to be sent
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Builds
      - Transaction
      - That
      - Sends
      - NTP1
      - Token
  /ntp1/burntoken:
    post:
      summary: Builds a transaction that burns an NTP1 Token
      description: Builds an unsigned raw transaction that burns an NTP1 token on
        the Neblio blockchain.
      operationId: burnToken
      x-api-path-slug: ntp1burntoken-post
      parameters:
      - in: body
        name: body
        description: Object representing the token to be burned
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Builds
      - Transaction
      - That
      - Burns
      - NTP1
      - Token
  /ins/tx/send:
    post:
      summary: Broadcasts a signed raw transaction to the network (not NTP1 specific)
      description: Broadcasts a signed raw transaction to the network. If successful
        returns the txid of the broadcast trasnaction.
      operationId: sendTx
      x-api-path-slug: instxsend-post
      parameters:
      - in: body
        name: body
        description: Object representing a transaction to broadcast
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Broadcasts
      - Signed
      - Raw
      - Transaction
      - To
      - Network
      - (not
      - NTP1
      - Specific)
  /ins/block/{blockhash}:
    get:
      summary: Returns information regarding a Neblio block
      description: Returns blockchain data for a given block based upon the block
        hash
      operationId: getBlock
      x-api-path-slug: insblockblockhash-get
      parameters:
      - in: path
        name: blockhash
        description: Block Hash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Information
      - Regarding
      - Neblio
      - Block
  /ins/block-index/{blockindex}:
    get:
      summary: Returns block hash of block
      description: Returns the block hash of a block at a given block index
      operationId: getBlockIndex
      x-api-path-slug: insblockindexblockindex-get
      parameters:
      - in: path
        name: blockindex
        description: Block Index
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Block
      - Hash
      - Of
      - Block
  /ins/tx/{txid}:
    get:
      summary: Returns transaction object
      description: Returns NEBL transaction object representing a NEBL transaction
      operationId: getTx
      x-api-path-slug: instxtxid-get
      parameters:
      - in: path
        name: txid
        description: Transaction ID
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Transaction
      - Object
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