{
  "info": {
    "name": "Blockchain Info Raw Address",
    "_postman_id": "c83dcf6c-1712-4377-ba5d-2e18f375c4ba",
    "description": "Returns a single blockchain address.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "56cfd9c5-aa33-4fea-b938-83cd30231691",
          "name": "getRawAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "blockchain.info",
              "path": [
                "rawaddr/:bitcoin_address"
              ],
              "variable": [
                {
                  "id": "bitcoin_address",
                  "value": "bitcoin_address",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a single blockchain address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5937e33d-ac84-4dba-a2e2-4d594d9bb450"
            }
          ]
        }
      ]
    }
  ]
}