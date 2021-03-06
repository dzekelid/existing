swagger: "2.0"
x-collection-name: DigitalOcean
x-complete: 1
info:
  title: DigitalOcean API-V2
  description: -api-v2-introductionwelcome-to-the-digitalocean-api-documentation-the-digitalocean-api-allows-you-to-manage-droplets-and-resources-within-the-digitalocean-cloud-in-a-simple-programmatic-way-using-conventional-http-requests--the-endpoints-are-intuitive-and-powerful-allowing-you-to-easily-make-calls-to-retrieve-information-or-to-execute-actions-all-of-the-functionality-that-you-are-familiar-with-in-the-digitalocean-control-panel-is-also-available-through-the-api-allowing-you-to-script-the-complex-actions-that-your-situation-requires-the-api-documentation-will-start-with-a-general-overview-about-the-design-and-technology-that-has-been-implemented-followed-by-reference-information-about-specific-endpoints-requestsany-tool-that-is-fluent-in-http-can-communicate-with-the-api-simply-by-requesting-the-correct-uri--requests-should-be-made-using-the-https-protocol-so-that-traffic-is-encrypted--the-interface-responds-to-different-methods-depending-on-the-action-required-methodusagegetfor-simple-retrieval-of-information-about-your-account-droplets-or-environment-you-should-use-the-get-method--the-information-you-request-will-be-returned-to-you-as-a-json-object-the-attributes-defined-by-the-json-object-can-be-used-to-form-additional-requests--any-request-using-the-get-method-is-readonly-and-will-not-affect-any-of-the-objects-you-are-querying-deleteto-destroy-a-resource-and-remove-it-from-your-account-and-environment-the-delete-method-should-be-used--this-will-remove-the-specified-object-if-it-is-found--if-it-is-not-found-the-operation-will-return-a-response-indicating-that-the-object-was-not-found-this-idempotency-means-that-you-do-not-have-to-check-for-a-resources-availability-prior-to-issuing-a-delete-command-the-final-state-will-be-the-same-regardless-of-its-existence-putto-update-the-information-about-a-resource-in-your-account-the-put-method-is-available-like-the-delete-method-the-put-method-is-idempotent--it-sets-the-state-of-the-target-using-the-provided-values-regardless-of-their-current-values--requests-using-the-put-method-do-not-need-to-check-the-current-attributes-of-the-object-postto-create-a-new-object-your-request-should-specify-the-post-method-the-post-request-includes-all-of-the-attributes-necessary-to-create-a-new-object--when-you-wish-to-create-a-new-object-send-a-post-request-to-the-target-endpoint-headfinally-to-retrieve-metadata-information-you-should-use-the-head-method-to-get-the-headers--this-returns-only-the-header-of-what-would-be-returned-with-an-associated-get-request-response-headers-contain-some-useful-information-about-your-api-access-and-the-results-that-are-available-for-your-request-for-instance-the-headers-contain-your-current-ratelimit-value-and-the-amount-of-time-available-until-the-limit-resets--it-also-contains-metrics-about-the-total-number-of-objects-found-pagination-information-and-the-total-content-length-
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