---
swagger: "2.0"
x-collection-name: SAP
x-complete: 0
info:
  title: SAP Translation Hub The '/translate' resource enables you to get translations
    of English short texts that exist in SAP Translation Hub.
  description: Provides translations of short texts based on a combination of existing
    texts and their translations that are used in SAP products and machine translation
    capabilities.
  contact:
    name: SAP Translation Hub team
    email: translationhub@sap.com
  version: 1.0.0
host: sandbox.api.sap.com
basePath: /translationhub/api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /translate:
    post:
      summary: The '/translate' resource enables you to get translations of English
        short texts that exist in SAP Translation Hub.
      description: Provides translations of short texts based on a combination of
        existing texts and their translations that are used in SAP products and machine
        translation capabilities.
      operationId: provides-translations-of-short-texts-based-on-a-combination-of-existing-texts-and-their-translations
      x-api-path-slug: translate-post
      parameters:
      - in: header
        name: Content-Type
        description: Specifies the nature of the data in the body so that the receiving
          agent can process the data accordingly
      - in: body
        name: translate
        description: The JSON request contains an array of ```units``` JSON objects
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - The
      - ""
      - Translate
      - Resource
      - Enables
      - You
      - To
      - Get
      - Translations
      - Of
      - English
      - Short
      - Texts
      - That
      - Exist
      - In
      - SAP
      - Translation
      - Hub
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