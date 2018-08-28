---
swagger: "2.0"
x-collection-name: Quovo
x-complete: 0
info:
  title: Quovo Update an existing webhook
  description: Used to update an existing webhook.
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tokens:
    delete:
      summary: Delete an existing access token
      description: Deletes an Access Token.
      operationId: TokensDelete
      x-api-path-slug: tokens-delete
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
      - Existing
      - Access
      - Token
  /webhooks:
    put:
      summary: Update an existing webhook
      description: Used to update an existing webhook.
      operationId: WebhooksPut
      x-api-path-slug: webhooks-put
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
      - Existing
      - Webhook
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