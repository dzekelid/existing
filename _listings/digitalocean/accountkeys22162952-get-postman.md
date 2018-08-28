{
  "info": {
    "name": "Digital Ocean Retrieve an existing Key",
    "_postman_id": "37a2ba11-3e71-42ee-9687-bd9b23f2553a",
    "description": "To show information about a key, send a GET request to /v2/account/keys/$KEY_ID or /v2/account/keys/$KEY_FINGERPRINT.\r\n\r\nThe response will be a JSON object with a key called _ssh_key_.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Retrieve",
      "item": [
        {
          "id": "5d828382-47d5-4f48-88e3-9f9c4fbf79b6",
          "name": "Certificates892071a0Bb9549bc80213afd67a210bfGet",
          "request": {
            "url": "http://example.com/certificates/892071a0-bb95-49bc-8021-3afd67a210bf",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "To show information about an existing certificate, send a GET request to /v2/certificates/$CERTIFICATE_ID.\r\n\r\nThe response will be a JSON object with a certificate key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "288b39b4-db64-4218-ab92-722012008074"
            }
          ]
        },
        {
          "id": "9d9bf650-4965-4f5f-94b0-0e5fd0b2166d",
          "name": "Images63261821Get",
          "request": {
            "url": "http://example.com/images/63261821",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve information about an image (public or private), send a GET request to /v2/images/$IMAGE_ID.\r\n\r\nThe response will be a JSON object with a key called image. The value of this will be an image object containing the standard image attributes:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd50b0d1-6e26-4164-a823-1b37f868a726"
            }
          ]
        },
        {
          "id": "0a33b03b-13ae-488e-823a-63b951437d36",
          "name": "AccountKeys22162952Get",
          "request": {
            "url": "http://example.com/account/keys/22162952",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "To show information about a key, send a GET request to /v2/account/keys/$KEY_ID or /v2/account/keys/$KEY_FINGERPRINT.\r\n\r\nThe response will be a JSON object with a key called _ssh_key_."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69bb425b-41a5-4fba-b711-3f4c11070f1c"
            }
          ]
        }
      ]
    }
  ]
}