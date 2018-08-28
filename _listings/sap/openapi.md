swagger: "2.0"
x-collection-name: SAP
x-complete: 1
info:
  title: SAP Translation Hub
  description: to-provide-users-of-software-in-a-global-market-with-texts-in-their-own-language-translations-are-required--sap-translation-hub-enables-you-to-draw-on-saps-translation-experience-across-multiple-products-and-languages-to-propose-translations-for-short-texts-
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