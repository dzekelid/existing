{
  "info": {
    "name": "Aspose.Storage API Get Storage Exist Path",
    "_postman_id": "27f02fea-f413-46f5-a296-cd98f5641de2",
    "description": "The controller checks that the file or folder exists in the service file storage.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Storage",
      "item": [
        {
          "id": "0198cad6-ff2a-4461-9510-cd17eb655a13",
          "name": "getStorageDisc",
          "request": {
            "url": "http://api.aspose.com/v1.1/storage/disc",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The resource represents information about users application disc usage (size in bytes"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc585e6c-d1a2-48b3-ae6a-3a1c57db987e"
            }
          ]
        },
        {
          "id": "9ac52804-b7db-4c1e-b639-0bf4c690422e",
          "name": "getStorageExistPath",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.aspose.com",
              "path": [
                "v1.1",
                "storage/exist/:path"
              ],
              "variable": [
                {
                  "id": "path",
                  "value": "path",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The controller checks that the file or folder exists in the service file storage."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bdd1840c-7232-4c50-b77c-696cadcaf69b"
            }
          ]
        }
      ]
    }
  ]
}