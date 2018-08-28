---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Modify an existing product image
  description: Modify an existing product image.
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/metafields/33145232974.json:
    put:
      summary: Update an existing store metafield.
      description: Update an existing store metafield..
      operationId: putAdminMetafields33145232974.json
      x-api-path-slug: adminmetafields33145232974-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Existing
      - Store
      - Metafield
  /admin/orders/4602125518/risks/8609858574.json:
    put:
      summary: Update an existing risk detail line on an order
      description: Update an existing risk detail line on an order.
      operationId: putAdminOrders4602125518Risks8609858574.json
      x-api-path-slug: adminorders4602125518risks8609858574-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Existing
      - Risk
      - Detail
      - Line
      - "On"
      - Order
  /admin/variants/34705478094.json:
    put:
      summary: Update an existing product variant
      description: Update an existing product variant.
      operationId: putAdminVariants34705478094.json
      x-api-path-slug: adminvariants34705478094-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Existing
      - Product
      - Variant
  /admin/orders.json:
    post:
      summary: Create a pending order with an existing customer
      description: Create a pending order with an existing customer.
      operationId: postAdminOrders.json
      x-api-path-slug: adminorders-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Pending
      - Order
      - Existing
      - Customer
  /admin/themes/110163843/assets.json:
    put:
      summary: Change an existing liquid template's value
      description: Change an existing liquid template's value.
      operationId: putAdminThemes110163843Assets.json
      x-api-path-slug: adminthemes110163843assets-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Change
      - Existing
      - Liquid
      - Templates
      - Value
  /admin/products/7990943555/images/19489404942.json:
    put:
      summary: Modify an existing product image
      description: Modify an existing product image.
      operationId: putAdminProducts7990943555Images19489404942.json
      x-api-path-slug: adminproducts7990943555images19489404942-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Modify
      - Existing
      - Product
      - Image
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