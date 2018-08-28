---
swagger: "2.0"
x-collection-name: Square
x-complete: 0
info:
  title: Square Connect API Deletes an existing fee (tax).
  description: Deletes an existing fee (tax).
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{location_id}/categories/{category_id}:
    delete:
      summary: Deletes an existing item category.
      description: Deletes an existing item category.
      operationId: DeleteCategory
      x-api-path-slug: v1location-idcategoriescategory-id-delete
      parameters:
      - in: path
        name: category_id
        description: The ID of the category to delete
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Item
      - Category
    put:
      summary: Modifies the details of an existing item category.
      description: Modifies the details of an existing item category.
      operationId: UpdateCategory
      x-api-path-slug: v1location-idcategoriescategory-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: category_id
        description: The ID of the category to edit
      - in: path
        name: location_id
        description: The ID of the categorys associated location
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Existing
      - Item
      - Category
  /v1/{location_id}/discounts/{discount_id}:
    delete:
      summary: Deletes an existing discount.
      description: Deletes an existing discount.
      operationId: DeleteDiscount
      x-api-path-slug: v1location-iddiscountsdiscount-id-delete
      parameters:
      - in: path
        name: discount_id
        description: The ID of the discount to delete
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Discount
    put:
      summary: Modifies the details of an existing discount.
      description: Modifies the details of an existing discount.
      operationId: UpdateDiscount
      x-api-path-slug: v1location-iddiscountsdiscount-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: discount_id
        description: The ID of the discount to edit
      - in: path
        name: location_id
        description: The ID of the categorys associated location
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Existing
      - Discount
  /v1/{location_id}/fees/{fee_id}:
    delete:
      summary: Deletes an existing fee (tax).
      description: Deletes an existing fee (tax).
      operationId: DeleteFee
      x-api-path-slug: v1location-idfeesfee-id-delete
      parameters:
      - in: path
        name: fee_id
        description: The ID of the fee to delete
      - in: path
        name: location_id
        description: The ID of the fees associated location
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Fee
      - (tax)
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