{
  "info": {
    "name": "Cryptagio Get Ticker",
    "_postman_id": "5d434c21-2013-4138-9e63-97920ae507fd",
    "description": "Get ticker of all markets..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "52c1bb97-8a12-4072-a81f-33efc9c96c50",
          "name": "getInfo",
          "request": {
            "url": "{{default}}/info",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get information.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7062c3c-d202-450d-b0d1-453722671fa8"
            }
          ]
        },
        {
          "id": "03883eab-76bb-49c8-a1a0-136d39f4ac81",
          "name": "getTicker",
          "request": {
            "url": "{{default}}/ticker",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get ticker of all markets.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3a4ca40-e211-4797-898f-9ee88cf9d995"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/"
    }
  ]
}