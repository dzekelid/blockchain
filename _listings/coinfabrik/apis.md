---
name: CoinFabrik
x-slug: coinfabrik
description: Our smart contract development and full stack blockchain development
  services are supported by more than 20 years of experience building and reviewing
  secure applications. CoinFabrik is a full stack blockchain development company.
  Our expertise range from extending cryptocurrency nodes like Bitcoin and Ethereum
  to providing high level APIs and UIs.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
x-kinRank: "7"
x-alexaRank: "970321"
tags: Blockchain
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/apis.md
specificationVersion: "0.14"
apis:
- name: Coinbase API - Show a user
  x-api-slug: usersuser-id-get
  description: "Get any user\u2019s public information with their ID."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/usersuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/usersuser-id-get-openapi.md
- name: Coinbase API - Show current user
  x-api-slug: user-get
  description: "Get current user\u2019s public information. To get user\u2019s email
    or private information, use permissions wallet:user:email and wallet:user:read."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/user-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/user-get-openapi.md
- name: Coinbase API - Update current user
  x-api-slug: user-put
  description: Modify current user and their preferences.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/user-put-openapi.md
- name: Coinbase API - Show authorization information
  x-api-slug: userauth-get
  description: "Get current user\u2019s authorization information including granted
    scopes and send limits when using OAuth2 authentication."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/userauth-get-openapi.md
- name: Coinbase API - List accounts
  x-api-slug: accounts-get
  description: "Lists current user\u2019s accounts to which the authentication method
    has access to."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/accounts-get-openapi.md
- name: Coinbase API - Create account
  x-api-slug: accounts-post
  description: Creates a new account for user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/accounts-post-openapi.md
- name: Coinbase API - Show an account
  x-api-slug: accountsaccount-id-get
  description: "Show current user\u2019s account. To access user\u2019s primary account,
    primary keyword can be used instead of the account id in the URL."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/accountsaccount-id-get-openapi.md
- name: Coinbase API - Update account
  x-api-slug: accountsaccount-id-put
  description: "Modifies user\u2019s account name."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/accountsaccount-id-put-openapi.md
- name: Coinbase API - Delete account
  x-api-slug: accountsaccount-id-delete
  description: "Removes user\u2019s account. In order to remove an account it can\u2019t
    be\n\n- Primary account\n- Account with non-zero balance\n- Fiat account\n- Vault
    with a pending withdrawal"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/accountsaccount-id-delete-openapi.md
- name: Coinbase API - Set account as primary
  x-api-slug: accountsaccount-idprimary-get
  description: Promote an account as primary account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/accountsaccount-idprimary-get-openapi.md
- name: Coinbase API - List addresses
  x-api-slug: accountsaccount-idaddresses-get
  description: |-
    Lists addresses for an account.

    *Important*: Addresses should be considered one time use only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/accountsaccount-idaddresses-get-openapi.md
- name: Coinbase API - Create address
  x-api-slug: accountsaccount-idaddresses-post
  description: "Creates a new address for an account. As all the arguments are optinal,
    it\u2019s possible just to do a empty POST which will create a new address. This
    is handy if you need to create new receive addresses for an account on-demand.\nAddresses
    can be created for all account types. With fiat accounts, funds will be received
    with Instant Exchange."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/accountsaccount-idaddresses-post-openapi.md
- name: Coinbase API - Show an address
  x-api-slug: accountsaccount-idaddressesaddress-id-get
  description: "Show an individual address for an account.\nRegular bitcoin address
    can be used in place of address_id but the address has to be associated to the
    correct account.\n  \n*Important* Addresses should be considered one time use
    only."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/accountsaccount-idaddressesaddress-id-get-openapi.md
- name: "Coinbase API - List address\u2019s transactions"
  x-api-slug: accountsaccount-idaddressesaddress-idtransactions-get
  description: list transactions that have been sent to a specific address. Regular
    bitcoin address can be used in place of address_id but the address has to be associated
    to the correct account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/accountsaccount-idaddressesaddress-idtransactions-get-openapi.md
- name: Coinbase API - List transactions
  x-api-slug: accountsaccount-idtransactions-get
  description: "Lists account\u2019s transactions. See Transaction resource for more
    information."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/accountsaccount-idtransactions-get-openapi.md
- name: Coinbase API - Send or request money
  x-api-slug: accountsaccount-idtransactions-post
  description: |-
    Type=send
    =========

    Send funds to a bitcoin address or email address. No transaction fees are required for off blockchain transactions, and Coinbase waives fees for on-blockchain transactions greater than 0.0001 BTC, up to a threshold of 25 per day. Read more about free transactions.

    When used with OAuth2 authentication, this endpoint requires two factor authentication unless used with wallet:transactions:send:bypass-2fa scope.

    If the user is able to buy bitcoin, they can send funds from their fiat account using instant exchange feature. Buy fees will be included in the created transaction and the recipient will receive the user defined amount.

    To create a multisig transaction, visit Multisig documentation.

    Type=request
    ============

    Requests money from an email address.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/accountsaccount-idtransactions-post-openapi.md
- name: Coinbase API - Show a transaction
  x-api-slug: accountsaccount-idtransactionstransaction-id-get
  description: Show an individual transaction for an account. See Transaction resource
    for more information.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/accountsaccount-idtransactionstransaction-id-get-openapi.md
- name: Coinbase API - Cancel request money
  x-api-slug: accountsaccount-idtransactionstransaction-id-delete
  description: Lets a user cancel a money request. Money requests can be canceled
    by the sender or the recipient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/accountsaccount-idtransactionstransaction-id-delete-openapi.md
- name: Coinbase API - Complete request money
  x-api-slug: accountsaccount-idtransactionstransaction-idcomplete-post
  description: Lets the recipient of a money request complete the request by sending
    money to the user who requested the money. This can only be completed by the user
    to whom the request was made, not the user who sent the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/accountsaccount-idtransactionstransaction-idcomplete-post-openapi.md
- name: Coinbase API - Re-send request money
  x-api-slug: accountsaccount-idtransactionstransaction-idresend-post
  description: Lets the user resend a money request. This will notify recipient with
    a new email.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coinfabrik.png
  humanURL: https://www.coinfabrik.com
  baseURL: https://api.coinbase.com//v2
  tags: SaaS, Blockchain, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/coinfabrik/accountsaccount-idtransactionstransaction-idresend-post-openapi.md
x-common:
- type: x-blog-rss
  url: https://blog.coinfabrik.com/feed/
- type: x-github
  url: https://github.com/CoinFabrik
- type: x-openapi
  url: https://raw.githubusercontent.com/CoinFabrik/coinbase-api-swagger/master/swagger.json
- type: x-api-gallery
  url: http://codefresh.api.gallery.streamdata.io
- type: x-api-stack
  url: http://coinfabrik.stack.network
- type: x-blog
  url: https://blog.coinfabrik.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/coinfabrik
- type: x-twitter
  url: https://twitter.com/coinfabrik
- type: x-website
  url: https://www.coinfabrik.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---