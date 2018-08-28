---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Add a new contact to the given auction Role or edit an existing contact
  version: 1.0.0
  description: Add a new contact to the given auction role or edit an existing contact.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/auction/savecontact:
    post:
      summary: Add a new contact to the given auction Role or edit an existing contact
      description: Add a new contact to the given auction role or edit an existing
        contact.
      operationId: Auction_SaveAuctionContactBysaveContactDataContract
      x-api-path-slug: apiauctionsavecontact-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: saveContactDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Contact
      - To
      - Given
      - Auction
      - Role
      - Edit
      - Existing
      - Contact
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