---
name: MasterCard
x-slug: mastercard
description: Mastercard is a leading global payments & technology company that connects
  consumers, businesses, merchants, issuers & governments around the world.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
x-kinRank: "9"
x-alexaRank: "48280"
tags: Blockchain
created: "2018-08-25"
modified: "2018-08-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/apis.md
specificationVersion: "0.14"
apis:
- name: MasterCard - Get Status
  x-api-slug: status-get
  description: |-
    Gets general metadata about the current state of the blockchain network.
    Useful for building dashboards.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
  humanURL: https://developer.mastercard.com/
  baseURL: https://eas5stl0.mastercard.int:13046//z0/core/v1
  tags: Shopping, Commerce, Hosting, Finance, Merchant, Merchants, Coupons, Shopping,
    Offers, Payments, Finance, Target, Stack Network, Stack, Blockchain, Blockchains,
    Financial Services, Technology, API Provider, Profiles, Payments, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/status-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/status-get-openapi.md
- name: MasterCard - Get Node
  x-api-slug: node-get
  description: |-
    By default, this call gets information about your local node and its
    connections. The `scope` parameter enabled this query to be extended
    to get further information about nodes that are visible to your node.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
  humanURL: https://developer.mastercard.com/
  baseURL: https://eas5stl0.mastercard.int:13046//z0/core/v1
  tags: Shopping, Commerce, Hosting, Finance, Merchant, Merchants, Coupons, Shopping,
    Offers, Payments, Finance, Target, Stack Network, Stack, Blockchain, Blockchains,
    Financial Services, Technology, API Provider, Profiles, Payments, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/node-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/node-get-openapi.md
- name: MasterCard - Get Node Address
  x-api-slug: nodeaddress-get
  description: |-
    Information about a specific node may be retrieved by its address.
    This is useful when navigating the network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
  humanURL: https://developer.mastercard.com/
  baseURL: https://eas5stl0.mastercard.int:13046//z0/core/v1
  tags: Shopping, Commerce, Hosting, Finance, Merchant, Merchants, Coupons, Shopping,
    Offers, Payments, Finance, Target, Stack Network, Stack, Blockchain, Blockchains,
    Financial Services, Technology, API Provider, Profiles, Payments, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/nodeaddress-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/nodeaddress-get-openapi.md
- name: MasterCard - Get App
  x-api-slug: appid-get
  description: |-
    Information about an application referenced by the `id` parameter. If
    you are permissioned to that application, this will also return the
    message definitions you will need to comply with to issue valid transaction
    entries for that application.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
  humanURL: https://developer.mastercard.com/
  baseURL: https://eas5stl0.mastercard.int:13046//z0/core/v1
  tags: Shopping, Commerce, Hosting, Finance, Merchant, Merchants, Coupons, Shopping,
    Offers, Payments, Finance, Target, Stack Network, Stack, Blockchain, Blockchains,
    Financial Services, Technology, API Provider, Profiles, Payments, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/appid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/appid-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://mapquest.api.gallery.streamdata.io
- type: x-api-stack
  url: http://mastercard.stack.network
- type: x-base
  url: https://api.simplify.com
- type: x-blog
  url: https://developer.mastercard.com/portal/display/blogs/Developer+Blogs
- type: x-crunchbase
  url: https://crunchbase.com/organization/mastercard
- type: x-crunchbase
  url: http://www.crunchbase.com/company/mastercard
- type: x-github
  url: https://github.com/MasterCard
- type: x-website
  url: https://developer.mastercard.com/
- type: x-twitter
  url: https://twitter.com/AskMastercard
- type: x-twitter
  url: https://twitter.com/MasterCardDev
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---