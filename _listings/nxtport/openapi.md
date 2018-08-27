swagger: "2.0"
x-collection-name: NxtPort
x-complete: 1
info:
  title: Portcall+ API (sandbox)
  description: portplus-api
  version: 1.0.0
host: api-sb.nxtport.eu
basePath: /PortCallPlus/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/events/:
    post:
      summary: Create an Event
      description: |-
        Used to create an event for a container at a specific location and time.
        Each event is defined by a type.
        Currently a limited number of events (pickup and availability) are supported, but this may be extended with e.g. passage events.
        There are 2 ways to refer to a Container: by means of its id as defined in the Blockchain (this requires recording these ids in your app), or by means of a combination of the blNumber and isoNumber. Similarly, locations can be specified in 2 ways: by means of their id as defined in the Blockchain or by means of their name. In the latter case the name must be defined in a mapping   file for the Organization you - as a user- belong to. Also note that the container may not yet be known in the Blockchain at the time
        an availability event is created!
      operationId: postApiV1Events
      x-api-path-slug: apiv1events-post
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Event