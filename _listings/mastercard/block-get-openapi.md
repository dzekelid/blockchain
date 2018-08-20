---
swagger: "2.0"
x-collection-name: MasterCard
x-complete: 0
info:
  title: Mastercard Get Block
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
  version: 1.0.0
host: eas5stl0.mastercard.int:13046
basePath: /z0/core/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /status:
    get:
      summary: Get Status
      description: |-
        Gets general metadata about the current state of the blockchain network.
        Useful for building dashboards.
      operationId: getStatus
      x-api-path-slug: status-get
      parameters:
      - in: header
        name: MCWSSAML
        description: SAML Authorization
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Status
  /node:
    get:
      summary: Get Node
      description: |-
        By default, this call gets information about your local node and its
        connections. The `scope` parameter enabled this query to be extended
        to get further information about nodes that are visible to your node.
      operationId: getNode
      x-api-path-slug: node-get
      parameters:
      - in: header
        name: MCWSSAML
        description: SAML Authorization
      - in: query
        name: scope
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Node
  /node/{address}:
    get:
      summary: Get Node Address
      description: |-
        Information about a specific node may be retrieved by its address.
        This is useful when navigating the network.
      operationId: getNodeAddress
      x-api-path-slug: nodeaddress-get
      parameters:
      - in: path
        name: address
      - in: header
        name: MCWSSAML
        description: SAML Authorization
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Node
      - Address
  /app/{id}:
    get:
      summary: Get App
      description: |-
        Information about an application referenced by the `id` parameter. If
        you are permissioned to that application, this will also return the
        message definitions you will need to comply with to issue valid transaction
        entries for that application.
      operationId: getApp
      x-api-path-slug: appid-get
      parameters:
      - in: path
        name: id
      - in: header
        name: MCWSSAML
        description: SAML Authorization
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - App
    post:
      summary: Add App
      description: |-
        When you are permissioned onto the network, you will be issued one or
        more `id`s to use. You may then send or update configurations of the
        transaction message types you wish to use. These are specified using
        Protocol Buffer version 3 files as specified
        [here](https://developers.google.com/protocol-buffers/docs/proto3)
        This specification may be sent either as the canonical JSON transform
        or the native `.proto` file encoded as hex, base58 or base64.
      operationId: postApp
      x-api-path-slug: appid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: MCWSSAML
        description: SAML Authorization
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - App
  /address/{address}:
    get:
      summary: Get Address Address
      description: |-
        Information about a particular address on the network. Note that this
        call may return information about a blockchain node or a signing entity.
        Also, the level of detail returned will vary depending on your permissions
        for the query target.
      operationId: getAddressAddress
      x-api-path-slug: addressaddress-get
      parameters:
      - in: path
        name: address
      - in: header
        name: MCWSSAML
        description: SAML Authorization
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Address
      - Address
  /block:
    get:
      summary: Get Block
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
      operationId: getBlock
      x-api-path-slug: block-get
      parameters:
      - in: query
        name: from
        description: Specify the starting slot to return
      - in: header
        name: MCWSSAML
        description: SAML Authorization
      - in: query
        name: to
        description: Specify the last slot to return
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Block
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