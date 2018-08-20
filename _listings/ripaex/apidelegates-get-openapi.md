---
swagger: "2.0"
x-collection-name: RipaEx
x-complete: 0
info:
  title: RipaEx Delegates
  description: Get all delegates.
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
  /api/accounts/delegates/fee:
    get:
      summary: Accounts Delegates Fee
      description: Get the delegate fee of an account.
      operationId: accounts.getDelegatesFee
      x-api-path-slug: apiaccountsdelegatesfee-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Accounts
      - Delegates
      - Fee
  /api/accounts/delegates:
    get:
      summary: Accounts Delegates
      description: Get the delegates of an account.
      operationId: accounts.getDelegates
      x-api-path-slug: apiaccountsdelegates-get
      parameters:
      - in: query
        name: address
        description: A valid RIPA Address
      - in: query
        name: limit
        description: An unsigned integer that specifies the maximum number of records
      - in: query
        name: offset
        description: An unsigned integer that specified the number of records to skip
      - in: query
        name: orderBy
        description: A string that specifies the column by which to sort the records
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Accounts
      - Delegates
    put:
      summary: Accounts Delegates
      description: Vote for a delegate by public key.
      operationId: accounts.addDelegates
      x-api-path-slug: apiaccountsdelegates-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Accounts
      - Delegates
  /api/accounts:
    get:
      summary: Accounts
      description: Returns account information of an address.
      operationId: accounts.getAccount
      x-api-path-slug: apiaccounts-get
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
  /api/accounts/getAllAccounts:
    get:
      summary: Accounts Get All Accounts
      description: Get a list of accounts.
      operationId: accounts.getAllAccounts
      x-api-path-slug: apiaccountsgetallaccounts-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Accounts
      - ""
      - ""
      - Accounts
  /api/accounts/top:
    get:
      summary: Accounts Top
      description: Get a list of top accounts.
      operationId: accounts.top
      x-api-path-slug: apiaccountstop-get
      parameters:
      - in: query
        name: limit
        description: An unsigned integer that specifies the maximum number of records
      - in: query
        name: offset
        description: An unsigned integer that specified the number of records to skip
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Accounts
      - Top
  /api/accounts/count:
    get:
      summary: Accounts Count
      description: Get the count of accounts.
      operationId: accounts.count
      x-api-path-slug: apiaccountscount-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Accounts
      - Count
  /api/blocks/get:
    get:
      summary: Blocks Get
      description: Get block by id.
      operationId: blocks.getBlock
      x-api-path-slug: apiblocksget-get
      parameters:
      - in: query
        name: id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
  /api/blocks:
    get:
      summary: Blocks
      description: Get all blocks.
      operationId: blocks.getBlocks
      x-api-path-slug: apiblocks-get
      parameters:
      - in: query
        name: generatorPublicKey
        description: A valid RIPA Public Key
      - in: query
        name: height
      - in: query
        name: limit
        description: An unsigned integer that specifies the maximum number of records
      - in: query
        name: offset
        description: An unsigned integer that specified the number of records to skip
      - in: query
        name: orderBy
        description: A string that specifies the column by which to sort the records
      - in: query
        name: previousBlock
      - in: query
        name: reward
      - in: query
        name: totalAmount
      - in: query
        name: totalFee
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
  /api/blocks/getEpoch:
    get:
      summary: Blocks Get Epoch
      description: Get the blockchain epoch.
      operationId: blocks.getEpoch
      x-api-path-slug: apiblocksgetepoch-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
      - ""
      - Epoch
  /api/blocks/getHeight:
    get:
      summary: Blocks Get Height
      description: Get the blockchain height.
      operationId: blocks.getHeight
      x-api-path-slug: apiblocksgetheight-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
      - ""
      - Height
  /api/blocks/getNethash:
    get:
      summary: Blocks Get Nethash
      description: Get the blockchain nethash.
      operationId: blocks.getNethash
      x-api-path-slug: apiblocksgetnethash-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
      - ""
      - Nethash
  /api/blocks/getFee:
    get:
      summary: Blocks Get Fee
      description: Get the transaction fee for sending "normal" transactions.
      operationId: blocks.getFee
      x-api-path-slug: apiblocksgetfee-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
      - ""
      - Fee
  /api/blocks/getFees:
    get:
      summary: Blocks Get Fees
      description: Get the network fees.
      operationId: blocks.getFees
      x-api-path-slug: apiblocksgetfees-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
      - ""
      - Fees
  /api/blocks/getMilestone:
    get:
      summary: Blocks Get Milestone
      description: Get the blockchain milestone.
      operationId: blocks.getMilestone
      x-api-path-slug: apiblocksgetmilestone-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
      - ""
      - Milestone
  /api/blocks/getReward:
    get:
      summary: Blocks Get Reward
      description: Get the blockchain reward.
      operationId: blocks.getReward
      x-api-path-slug: apiblocksgetreward-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
      - ""
      - Reward
  /api/blocks/getSupply:
    get:
      summary: Blocks Get Supply
      description: Get the blockchain supply.
      operationId: blocks.getSupply
      x-api-path-slug: apiblocksgetsupply-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
      - ""
      - Supply
  /api/blocks/getStatus:
    get:
      summary: Blocks Get Status
      description: Get the blockchain status.
      operationId: blocks.getStatus
      x-api-path-slug: apiblocksgetstatus-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
      - ""
      - Status
  /api/delegates/count:
    get:
      summary: Delegates Count
      description: Get the count of delegates.
      operationId: delegates.count
      x-api-path-slug: apidelegatescount-get
      parameters:
      - in: query
        name: address
        description: A valid RIPA Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Delegates
      - Count
  /api/delegates/search:
    get:
      summary: Delegates Search
      description: Search for specific delegates.
      operationId: delegates.search
      x-api-path-slug: apidelegatessearch-get
      parameters:
      - in: query
        name: limit
        description: An unsigned integer that specifies the maximum number of records
      - in: query
        name: q
        description: A search query
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Delegates
      - Search
  /api/delegates/voters:
    get:
      summary: Delegates Voters
      description: Get a list of voters for a delegate.
      operationId: delegates.getVoters
      x-api-path-slug: apidelegatesvoters-get
      parameters:
      - in: query
        name: publicKey
        description: A valid RIPA Public Key
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Delegates
      - Voters
  /api/delegates/get:
    get:
      summary: Delegates Get
      description: Get a single delegate.
      operationId: delegates.getDelegate
      x-api-path-slug: apidelegatesget-get
      parameters:
      - in: query
        name: publicKey
        description: A valid RIPA Public Key
      - in: query
        name: username
        description: A valid RIPA Delegate username
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Delegates
  /api/delegates:
    get:
      summary: Delegates
      description: Get all delegates.
      operationId: delegates.getDelegates
      x-api-path-slug: apidelegates-get
      parameters:
      - in: query
        name: limit
        description: An unsigned integer that specifies the maximum number of records
      - in: query
        name: offset
        description: An unsigned integer that specified the number of records to skip
      - in: query
        name: orderBy
        description: A string that specifies the column by which to sort the records
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Delegates
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