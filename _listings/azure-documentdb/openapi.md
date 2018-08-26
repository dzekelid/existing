---
swagger: "2.0"
x-collection-name: Azure DocumentDB
x-complete: 1
info:
  title: DocumentDB
  description: azure-documentdb-database-service-resource-provider-rest-api
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
---