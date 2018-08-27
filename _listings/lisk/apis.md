---
name: Lisk
x-slug: lisk
description: Lisk makes it easy for developers to build and deploy blockchain applications
  in JavaScript. Join the leading platform for world-changing dapps.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
x-kinRank: "7"
x-alexaRank: "145661"
tags: Blockchain
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/apis.md
specificationVersion: "0.14"
apis:
- name: 'Lisk API Documentation - '
  x-api-slug: spec-xswaggerpipe
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/spec-xswaggerpipe-openapi.md
- name: Lisk API Documentation - Submits signed transaction for processing
  x-api-slug: transactions-post
  description: |-
    Submits signed transaction object for processing by the transaction pool.
    Transaction objects can be generated locally either by using Lisk Commander or with Lisk Elements.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/transactions-post-openapi.md
- name: Lisk API Documentation - Requests transactions data
  x-api-slug: transactions-get
  description: Search for a specified transaction in the system.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/transactions-get-openapi.md
- name: Lisk API Documentation - Submits a signature object to sign multisignature
    transactions
  x-api-slug: signatures-post
  description: |-
    Submits signature to sign a multisignature transaction.
    Signature objects can be generated locally either by using Lisk Commander or with Lisk Elements.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/signatures-post-openapi.md
- name: Lisk API Documentation - Requests votes data for an account
  x-api-slug: votes-get
  description: |-
    *Attention: At least **one of the filter parameters must be provided.***
    Returns all votes placed by an account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/votes-get-openapi.md
- name: Lisk API Documentation - Requests voters data for a delegate
  x-api-slug: voters-get
  description: |-
    *Attention: At least **one of the filter parameters must be provided.***
    Returns all votes received by a delegate.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/voters-get-openapi.md
- name: Lisk API Documentation - Requests blocks data
  x-api-slug: blocks-get
  description: Search for a specified block in the system.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/blocks-get-openapi.md
- name: Lisk API Documentation - Requests forging stats by delegate
  x-api-slug: delegatesaddressforging-statistics-get
  description: |-
    By passing an existing delegate address and the desired unix timestamps, you can get its forging statistics within the specified timespan.
    If no timestamps are provided, it will use the timestamps from Lisk epoch to current date.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/delegatesaddressforging-statistics-get-openapi.md
- name: Lisk API Documentation - Requests next forgers data
  x-api-slug: delegatesforgers-get
  description: Returns a list of the next forgers in this delegate round.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/delegatesforgers-get-openapi.md
- name: Lisk API Documentation - Requests delegates data
  x-api-slug: delegates-get
  description: Search for a specified delegate in the system.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/delegates-get-openapi.md
- name: Lisk API Documentation - Requests unprocessed transactions data
  x-api-slug: nodetransactionsstate-get
  description: |-
    By specifying the state of the transactions, you get a list of unprocessed transactions matching this state.
    Search for specific transactions by providing the appropriate parameters.
    If you post a batch of transactions, they will appear in the unprocessed list after a small delay, depending on server load.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/nodetransactionsstate-get-openapi.md
- name: Lisk API Documentation - Toggles the forging status of a delegate
  x-api-slug: nodestatusforging-put
  description: |-
    *Attention! This is a **private endpoint only authorized to whitelisted IPs.**
    To edit the whitelist, please edit the `forging.access.whitelist` section in `config.json`*<br>
    Upon passing the correct password and publicKey, forging will be enabled or disabled for the delegate of this particular node.
    The password can be generated locally by encrypting your passphrase, either by using Lisk Commander or with Lisk Elements.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/nodestatusforging-put-openapi.md
- name: Lisk API Documentation - Requests forging status of a delegate
  x-api-slug: nodestatusforging-get
  description: |-
    *Attention! This is a **private endpoint only authorized to whitelisted IPs.**
    To edit the whitelist, please edit the `forging.access.whitelist` section in `config.json`*<br>
    Responds with the forging status of a delegate on a node.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/nodestatusforging-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/nodestatusforging-get-openapi.md
- name: Lisk API Documentation - Requests status data
  x-api-slug: nodestatus-get
  description: Returns all current status data of the node, e.g. height and broadhash.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/nodestatus-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/nodestatus-get-openapi.md
- name: Lisk API Documentation - Requests constants data
  x-api-slug: nodeconstants-get
  description: Returns all current constants data on the system, e.g. Lisk epoch time
    and version.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/nodeconstants-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/nodeconstants-get-openapi.md
- name: Lisk API Documentation - Requests peers data
  x-api-slug: peers-get
  description: Search for specified peers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/peers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/peers-get-openapi.md
- name: Lisk API Documentation - Requests dapps data
  x-api-slug: dapps-get
  description: Search for a specified dapp in the system.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/dapps-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/dapps-get-openapi.md
- name: Lisk API Documentation - Requests multisignature membership data
  x-api-slug: accountsaddressmultisignature-memberships-get
  description: Searches for the specified multisignature group and responds with a
    list of all members of this particular multisignature group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/accountsaddressmultisignature-memberships-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/accountsaddressmultisignature-memberships-get-openapi.md
- name: Lisk API Documentation - Requests multisignature groups data
  x-api-slug: accountsaddressmultisignature-groups-get
  description: Searches for the specified account in the system and responds with
    a list of the multisignature groups that this account is member of.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/accountsaddressmultisignature-groups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/accountsaddressmultisignature-groups-get-openapi.md
- name: Lisk API Documentation - Requests account data
  x-api-slug: accounts-get
  description: Search for matching accounts in the system.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/26631-lisk.jpg
  humanURL: https://lisk.io
  baseURL: https:////api
  tags: Technology, SaaS, Enterprise, Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/lisk/accounts-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://linkedin.api.gallery.streamdata.io
- type: x-crunchbase
  url: https://crunchbase.com/organization/lisk
- type: x-email
  url: support@lisk.io
- type: x-email
  url: dataprotection@lisk.io
- type: x-email
  url: help@lisk.io
- type: x-email
  url: business@lisk.io
- type: x-email
  url: events@lisk.io
- type: x-twitter
  url: https://twitter.com/LiskHQ
- type: x-website
  url: https://lisk.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---