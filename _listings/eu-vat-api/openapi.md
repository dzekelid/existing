swagger: "2.0"
x-collection-name: EU VAT API
x-complete: 1
info:
  title: VAT API
  description: a-developer-friendly-api-to-help-your-business-achieve-vat-compliance
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