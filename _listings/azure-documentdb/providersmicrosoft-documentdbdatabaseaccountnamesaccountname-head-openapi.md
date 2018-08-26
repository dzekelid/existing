---
swagger: "2.0"
x-collection-name: Azure DocumentDB
x-complete: 0
info:
  title: Azure DocumentDB API Database Accounts Check Name Exists
  description: Checks that the Azure DocumentDB account name already exists. A valid
    account name may contain only lowercase letters, numbers, and the '-' character,
    and must be between 3 and 50 characters.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /providers/Microsoft.DocumentDB/databaseAccountNames/{accountName}:
    head:
      summary: Database Accounts Check Name Exists
      description: Checks that the Azure DocumentDB account name already exists. A
        valid account name may contain only lowercase letters, numbers, and the '-'
        character, and must be between 3 and 50 characters.
      operationId: DatabaseAccounts_CheckNameExists
      x-api-path-slug: providersmicrosoft-documentdbdatabaseaccountnamesaccountname-head
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Database
      - Accounts
      - Checks
      - Name
      - Exists
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