---
swagger: "2.0"
x-collection-name: IBM Financial Crimes Insight for Insurance
x-complete: 1
info:
  title: Financial Crimes Insight for Insurance public REST APIs
  description: these-are-the-financial-crimes-insight-for-insurance-public-rest-apis-used-by-clients-to-access-the-fcii-capabilities
  version: 1.0.0
host: fcihost.ibm.com:9443
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ibm/fci/platform/fact/{type}/{remoteSystem}/{remoteKey}/assessments]:
    get:
      summary: Return the existing assessments for the object specified
      description: This service is used to return the existing assessments for the
        object specified.
      operationId: requestAssessmentValue
      x-api-path-slug: ibmfciplatformfacttyperemotesystemremotekeyassessments-get
      parameters:
      - in: query
        name: context
        description: The fraud context for which to return assessements
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: path
        name: remoteKey
        description: The combination of remoteSystem and remoteKey uniquely defines
          an object
      - in: path
        name: remoteSystem
        description: The combination of remoteSystem and remoteKey uniquely defines
          an object
      - in: path
        name: type
        description: Type of object; party, account, transaction, event, or other
          defined object type
      responses:
        200:
          description: OK
      tags:
      - Return
      - Existing
      - Assessmentsthe
      - Object
      - Specified
---