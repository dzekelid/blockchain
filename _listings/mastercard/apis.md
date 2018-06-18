---
name: MasterCard
x-slug: mastercard
description: Mastercard is a leading global payments & technology company that connects
  consumers, businesses, merchants, issuers & governments around the world.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
x-kinRank: "9"
x-alexaRank: "48280"
tags: Blockchain
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/apis.md
specificationVersion: "0.14"
apis:
- name: Mastercard Get Status
  x-api-slug: mastercard
  description: |-
    Gets general metadata about the current state of the blockchain network.
    Useful for building dashboards.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
  humanURL: https://developer.mastercard.com/
  baseURL: https://eas5stl0.mastercard.int:13046//z0/core/v1//status
  tags: Blockchain,Status
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/status-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/status-get-openapi.md
- name: Mastercard Get Node
  x-api-slug: mastercard
  description: |-
    By default, this call gets information about your local node and its
    connections. The `scope` parameter enabled this query to be extended
    to get further information about nodes that are visible to your node.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
  humanURL: https://developer.mastercard.com/
  baseURL: https://eas5stl0.mastercard.int:13046//z0/core/v1//node
  tags: Blockchain,Node
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/node-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/node-get-openapi.md
- name: Mastercard Get Node Address
  x-api-slug: mastercard
  description: |-
    Information about a specific node may be retrieved by its address.
    This is useful when navigating the network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
  humanURL: https://developer.mastercard.com/
  baseURL: https://eas5stl0.mastercard.int:13046//z0/core/v1//node/{address}
  tags: Blockchain,Node, Address
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/nodeaddress-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/nodeaddress-get-openapi.md
- name: Mastercard Get App
  x-api-slug: mastercard
  description: |-
    Information about an application referenced by the `id` parameter. If
    you are permissioned to that application, this will also return the
    message definitions you will need to comply with to issue valid transaction
    entries for that application.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
  humanURL: https://developer.mastercard.com/
  baseURL: https://eas5stl0.mastercard.int:13046//z0/core/v1//app/{id}
  tags: Blockchain,App
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/appid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/appid-get-openapi.md
- name: Mastercard Add App
  x-api-slug: mastercard
  description: |-
    When you are permissioned onto the network, you will be issued one or
    more `id`s to use. You may then send or update configurations of the
    transaction message types you wish to use. These are specified using
    Protocol Buffer version 3 files as specified
    [here](https://developers.google.com/protocol-buffers/docs/proto3)
    This specification may be sent either as the canonical JSON transform
    or the native `.proto` file encoded as hex, base58 or base64.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
  humanURL: https://developer.mastercard.com/
  baseURL: https://eas5stl0.mastercard.int:13046//z0/core/v1//app/{id}
  tags: Blockchain,App
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/appid-post-openapi.md
- name: Mastercard Get Address Address
  x-api-slug: mastercard
  description: |-
    Information about a particular address on the network. Note that this
    call may return information about a blockchain node or a signing entity.
    Also, the level of detail returned will vary depending on your permissions
    for the query target.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
  humanURL: https://developer.mastercard.com/
  baseURL: https://eas5stl0.mastercard.int:13046//z0/core/v1//address/{address}
  tags: Blockchain,Address, Address
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/addressaddress-get-openapi.md
- name: Mastercard Get Block
  x-api-slug: mastercard
  description: |-
    By default, this call returns the last confirmed block, since the `from`
    and `to` parameters will both default to the last confirmed slot number.
    To get a range of blocks, use the `from` and `to` parameters. Specifying
    only the `from` parameter will get a range of blocks up to the current slot.
    Note that this also means that specifying `to` without `from` will result
    in an error since that will mean a negative range.

    For each returned item, the data will contain header information from
    the block binary, and references to the block entries via the merkle roots.

    Note that the maximum range request allowed is 600 entries.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
  humanURL: https://developer.mastercard.com/
  baseURL: https://eas5stl0.mastercard.int:13046//z0/core/v1//block
  tags: Blockchain,Block
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/block-get-openapi.md
- name: Mastercard Get Block Key
  x-api-slug: mastercard
  description: |-
    A specific block may be retrieved by its hash key. This is useful when
    navigating the chain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
  humanURL: https://developer.mastercard.com/
  baseURL: https://eas5stl0.mastercard.int:13046//z0/core/v1//block/{key}
  tags: Blockchain,Block, Key
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/blockkey-get-openapi.md
- name: Mastercard Put Entry
  x-api-slug: mastercard
  description: |-
    Add a transaction entry for your application to the blockchain. Note that
    this entry must be a valid message according to the application configuration
    that you set up.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
  humanURL: https://developer.mastercard.com/
  baseURL: https://eas5stl0.mastercard.int:13046//z0/core/v1//entry
  tags: Blockchain,Entry
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/entry-put-openapi.md
- name: Mastercard Get Entry Key
  x-api-slug: mastercard
  description: |-
    Returns full detail of the value of the blockchain entry
    referenced by the specified key, if it has been previously recorded
    by your node's key-value store (database).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
  humanURL: https://developer.mastercard.com/
  baseURL: https://eas5stl0.mastercard.int:13046//z0/core/v1//entry/{key}
  tags: Blockchain,Entry, Key
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/entrykey-get-openapi.md
- name: Mastercard Add Support Encoding
  x-api-slug: mastercard
  description: |-
    A utility function that can be used temporarily if you don't have a
    library handy for a specific encoding. Provides transforms between
    Base-58, Base-64 and Hexadecimal encodings. You specify the input format
    and output format you wish, and a list of values to transcode.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
  humanURL: https://developer.mastercard.com/
  baseURL: https://eas5stl0.mastercard.int:13046//z0/core/v1//support/encoding
  tags: Blockchain,Support, Encoding
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/supportencoding-post-openapi.md
- name: Mastercard
  x-api-slug: mastercard
  description: Mastercard is a leading global payments & technology company that connects
    consumers, businesses, merchants, issuers & governments around the world.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/366-mastercard.jpg
  humanURL: https://developer.mastercard.com/
  baseURL: https://eas5stl0.mastercard.int:13046//z0/core/v1
  tags: Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/blockchain/master/_listings/mastercard/openapi.md
x-common:
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