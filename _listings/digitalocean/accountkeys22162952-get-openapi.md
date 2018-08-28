---
swagger: "2.0"
x-collection-name: DigitalOcean
x-complete: 0
info:
  title: Digital Ocean Retrieve an existing Key
  description: "To show information about a key, send a GET request to /v2/account/keys/$KEY_ID
    or /v2/account/keys/$KEY_FINGERPRINT.\r\n\r\nThe response will be a JSON object
    with a key called _ssh_key_."
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
  /certificates/892071a0-bb95-49bc-8021-3afd67a210bf:
    get:
      summary: Retrieve an existing certificate
      description: "To show information about an existing certificate, send a GET
        request to /v2/certificates/$CERTIFICATE_ID.\r\n\r\nThe response will be a
        JSON object with a certificate key."
      operationId: Certificates892071a0Bb9549bc80213afd67a210bfGet
      x-api-path-slug: certificates892071a0bb9549bc80213afd67a210bf-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Existing
      - Certificate
  /images/63261821:
    get:
      summary: Retrieve an existing Image by id
      description: "To retrieve information about an image (public or private), send
        a GET request to /v2/images/$IMAGE_ID.\r\n\r\nThe response will be a JSON
        object with a key called image. The value of this will be an image object
        containing the standard image attributes:"
      operationId: Images63261821Get
      x-api-path-slug: images63261821-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Existing
      - Image
      - By
      - Id
  /account/keys/22162952:
    get:
      summary: Retrieve an existing Key
      description: "To show information about a key, send a GET request to /v2/account/keys/$KEY_ID
        or /v2/account/keys/$KEY_FINGERPRINT.\r\n\r\nThe response will be a JSON object
        with a key called _ssh_key_."
      operationId: AccountKeys22162952Get
      x-api-path-slug: accountkeys22162952-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Existing
      - Key
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