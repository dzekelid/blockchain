---
swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 0
info:
  title: ChainGenie Refund buyer and stop trade (by Seller)
  description: "Seller can cancel the market trade after bid/buy by refunding the
    seller<br/>\r\nEscrow from buyer is returned back to the buyer<br/>\r\nEscrow
    from seller is returned back to the seller (optional: penalties can be imposed)<br/>\r\nEnd
    transaction state = Escrow returned, smart contract cancelled and become inactive<br/>"
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
  /tradechain/GetItemsFilterSort:
    post:
      summary: Report / list of marketplace transactions
      description: "Use a combination of fields to get any type of report.  Ex. send
        specific seller name or id to get active for sale items by seller; send specific
        filehash to get status of a particular item/invoice; send itemPartNum to get
        a list of all products of that partnumber and send sort order as itemValue
        ascending to cheapest top list) . . . \r\n-\tfilterField (accepted items below,
        default \u2013 none)\r\no\titemSellerId\r\no\titemSellerName\r\no\titemBuyerId\r\no\titemBuyerName\r\no\titemId\r\no\titemName\r\no\titemPartNum\r\no\tfileHash\r\no\tFileHash\r\n-\tsortField
        (accepted items below, default \u2013 itemValidUntil)\r\no\titemSellerId\r\no\titemSellerName\r\no\titemBuyerId\r\no\titemBuyerName\r\no\titemId\r\no\titemName\r\no\titemValue\r\no\titemPartNum\r\no\titemValidUntil\r\n-\tsortOrder
        (default \u2013 desc)\r\no\tasc\r\no\tdesc\r\n-\tonSaleOnly (default \u2013
        true, only if not \u201CInactive\u201D)\r\no\ttrue\r\no\tfalse\r\n-\tmaxPrice
        (double; default - 0)"
      operationId: TradechainGetItemsFilterSortPost
      x-api-path-slug: tradechaingetitemsfiltersort-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: filterField
      - in: formData
        name: filterValue
      - in: formData
        name: maxPrice
      - in: formData
        name: onSaleOnly
      - in: formData
        name: sortField
      - in: formData
        name: sortOrder
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Report
      - ""
      - ""
      - List
      - Of
      - Marketplace
      - Transactions
  /tradechain/WhoIsBuyer:
    post:
      summary: Get buyer information
      description: Get full information about the seller by providing the contract
        id.  Response will also include some contract details.
      operationId: TradechainWhoIsBuyerPost
      x-api-path-slug: tradechainwhoisbuyer-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemContractId
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Buyer
      - Information
  /tradechain/WhoIsSeller:
    post:
      summary: Get seller information
      description: Get full information about the seller by providing the contract
        id.  Response will also include some contract details.
      operationId: TradechainWhoIsSellerPost
      x-api-path-slug: tradechainwhoisseller-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemContractId
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Seller
      - Information
  /tradechain/GetFundsLockedInContract:
    post:
      summary: Get contract escrow details
      description: "Get contract escrow details -\n- Retrieves full information including
        but not limited to\n - Escrow amount in contract\n - Contract state \n - Buyer
        & Seller information\n - Links to contract / invoice documents\n - and other
        contract / sale specific information"
      operationId: TradechainGetFundsLockedInContractPost
      x-api-path-slug: tradechaingetfundslockedincontract-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemContractId
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Contract
      - Escrow
      - Details
  /tradechain/GetStateOfContract:
    post:
      summary: Get contract details & state
      description: "Get contract details & state\n- Provide full information including\n
        - Escrow amount in contract\n - Contract state \n - Buyer & Seller information\n
        - Links to contract / invoice documents\n - and other contract / sale specific
        information"
      operationId: TradechainGetStateOfContractPost
      x-api-path-slug: tradechaingetstateofcontract-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemContractId
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Contract
      - Details
      - '&'
      - State
  /tradechain/ConfirmReceived:
    post:
      summary: Delivery of item confirmed (by Buyer)
      description: "Delivery of item confirmed by the buyer \r\n-Escrow is fully sent
        to seller\r\n- End transaction state = TRANSACTION COMPLETE"
      operationId: TradechainConfirmReceivedPost
      x-api-path-slug: tradechainconfirmreceived-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemBuyerName
      - in: formData
        name: itemContractId
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Delivery
      - Of
      - Item
      - Confirmed
      - (by
      - Buyer)
  /tradechain/ConfirmRefund:
    post:
      summary: Refund buyer and stop trade (by Seller)
      description: "Seller can cancel the market trade after bid/buy by refunding
        the seller<br/>\r\nEscrow from buyer is returned back to the buyer<br/>\r\nEscrow
        from seller is returned back to the seller (optional: penalties can be imposed)<br/>\r\nEnd
        transaction state = Escrow returned, smart contract cancelled and become inactive<br/>"
      operationId: TradechainConfirmRefundPost
      x-api-path-slug: tradechainconfirmrefund-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemContractId
      - in: formData
        name: itemSellerName
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Refund
      - Buyer
      - Stop
      - Trade
      - (by
      - Seller)
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