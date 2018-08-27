---
swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 0
info:
  title: ChainGenie Check document exists on blockchain
  description: Check if your documents exists in the eth blockchain
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
  /tradechain/ConfirmPurchase:
    post:
      summary: Bid / buy listed item (by Buyer)
      description: "Bid / buy the item listed on the marketplace: <br/>\r\n- Buyer
        confirms interest in buying<br/>\r\n- Escrow from buyer added to value of
        contract<br/>\r\n- Invoice document is created with all details using invoice
        template<br/>\r\n- Invoice is added IPFS and invoice hash into blockchain<br/>\r\n-
        End transaction state = Trade is actively locked between the seller and buyer<br/>"
      operationId: TradechainConfirmPurchasePost
      x-api-path-slug: tradechainconfirmpurchase-post
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
      - Bid
      - ""
      - ""
      - Buy
      - Listed
      - Item
      - (by
      - Buyer)
  /tradechain/ConfirmAbort:
    post:
      summary: Remove Listing (by Seller)
      description: "Remove Listing (by Seller)<br/>\r\n- Seller cancels the market
        trade after listing but before bid/buy<br/>\r\n- Escrow from seller is returned
        back to the seller<br/>\r\n- End transaction state = Smart contract is rendered
        inactive<br/>"
      operationId: TradechainConfirmAbortPost
      x-api-path-slug: tradechainconfirmabort-post
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
      - Remove
      - Listing
      - (by
      - Seller)
  /tradechain/CreateTradeContract:
    post:
      summary: List product for sale
      description: "List product on marketplace: <br/>\r\n- Seller initiates sale
        - CreateTradeContract<br/>\r\n- Escrow from seller added for value of contract<br/>\r\n-
        End transaction state = Smart Contract Created<br/>"
      operationId: TradechainCreateTradeContractPost
      x-api-path-slug: tradechaincreatetradecontract-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemName
      - in: formData
        name: itemPartNum
      - in: formData
        name: itemSellerName
      - in: formData
        name: itemValidUntil
      - in: formData
        name: itemValue
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - List
      - Productsale
  /ethledger/gettrans:
    get:
      summary: Document transactions
      description: Displays all transactions connected to this project / smart contract
      operationId: EthledgerGettransGet
      x-api-path-slug: ethledgergettrans-get
      parameters:
      - in: header
        name: ApiKey
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Document
      - Transactions
  /ethledger/existsstr:
    post:
      summary: Check message exists on blockchain
      description: Check if your string exists in the eth blockchain
      operationId: EthledgerExistsstrPost
      x-api-path-slug: ethledgerexistsstr-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: str
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Check
      - Message
      - Exists
      - "On"
      - Blockchain
  /ethledger/poststr:
    post:
      summary: Write message to blockchain
      description: Post string hash into eth chain for POE (proof of existence)
      operationId: EthledgerPoststrPost
      x-api-path-slug: ethledgerpoststr-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: str
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Write
      - Message
      - To
      - Blockchain
  /ethledger/existshash:
    post:
      summary: Check hash exists on blockchain
      description: Check if your hash exists in the eth blockchain
      operationId: EthledgerExistshashPost
      x-api-path-slug: ethledgerexistshash-post
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
      - Check
      - Hash
      - Exists
      - "On"
      - Blockchain
  /ethledger/posthash:
    post:
      summary: Write hash to blockchain
      description: Post string hash into eth chain for POE (proof of existence)
      operationId: EthledgerPosthashPost
      x-api-path-slug: ethledgerposthash-post
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
      - Write
      - Hash
      - To
      - Blockchain
  /ethledger/getdocstate:
    post:
      summary: Get document status using hash
      description: Review the document status - existence, hash, block info, signatories,
        routing to users and details
      operationId: EthledgerGetdocstatePost
      x-api-path-slug: ethledgergetdocstate-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: strHash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Document
      - Status
      - Using
      - Hash
  /ethledger/signcert:
    post:
      summary: Sign document using hash (min fn; no return)
      description: Cryptographically sign the document and add the record to blockchain.  The
        document history and status is updated for querying.  The API call does not
        return any document properties.  This is a <b>minimalistic function</b> for
        stringing with other functions
      operationId: EthledgerSigncertPost
      x-api-path-slug: ethledgersigncert-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: strHash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Sign
      - Document
      - Using
      - Hash
      - (min
      - Fn;
      - "No"
      - Return)
  /ethledger/sendcert:
    post:
      summary: Send document using hash (min fn; no return)
      description: Route the document to a recipient.  The document history and status
        is updated for querying.  The API call does not return any document properties.  This
        is a <b>minimalistic function</b> for stringing with other functions
      operationId: EthledgerSendcertPost
      x-api-path-slug: ethledgersendcert-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: recipient
      - in: formData
        name: strHash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Send
      - Document
      - Using
      - Hash
      - (min
      - Fn;
      - "No"
      - Return)
  /ethledger/postdoc:
    post:
      summary: Post document to IPFS + blockchain
      description: Post document hash into eth chain for POE (proof of existence)
        and post the document into ipfs for safekeep!
      operationId: EthledgerPostdocPost
      x-api-path-slug: ethledgerpostdoc-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: files
      - in: formData
        name: filetypes
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Document
      - To
      - IPFS
      - +
      - Blockchain
  /ethledger/existsdoc:
    post:
      summary: Check document exists on blockchain
      description: Check if your documents exists in the eth blockchain
      operationId: EthledgerExistsdocPost
      x-api-path-slug: ethledgerexistsdoc-post
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
      - Check
      - Document
      - Exists
      - "On"
      - Blockchain
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