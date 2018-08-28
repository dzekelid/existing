---
swagger: "2.0"
x-collection-name: EU VAT API
x-complete: 0
info:
  title: EU VAT API Update an existing invoice
  description: Update an existing invoice.
  version: "1"
host: vatapi.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /invoice/{id}:
    put:
      summary: Update an existing invoice
      description: Update an existing invoice.
      operationId: invoice_update
      x-api-path-slug: invoiceid-put
      parameters:
      - in: body
        name: body
        description: Enter invoice data as JSON
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Enter an invoice id
      - in: header
        name: Response-Type
        description: The default response type is application/json if you would like
          to receive an XML response then set this to XML
      responses:
        200:
          description: OK
      tags:
      - Existing
      - Invoice
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