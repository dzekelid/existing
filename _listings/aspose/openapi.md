swagger: "2.0"
x-collection-name: Aspose
x-complete: 1
info:
  title: Aspose
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: api.aspose.com
basePath: /v1.1
paths:
  /storage/exist/{path}:
    get:
      summary: Get Storage Exist Path
      description: The controller checks that the file or folder exists in the service
        file storage.
      operationId: getStorageExistPath
      x-api-path-slug: storageexistpath-get
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Exist
      - Path