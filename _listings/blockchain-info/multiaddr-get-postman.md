{
  "info": {
    "name": "Blockchain Info Multi Adress",
    "_postman_id": "59362de6-0e0e-47ce-9620-b3f45723f41a",
    "description": "Returns multiple addresses",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "67a70ab3-b8e9-4a70-ba65-70f53b223a8d",
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
              "id": "ea481adc-f66d-4239-994d-f206548cd9f7"
            }
          ]
        },
        {
          "id": "6edadb4c-7298-404f-9cbc-ecd3c7eec54e",
          "name": "getMultipleAddresses",
          "request": {
            "url": "http://blockchain.info/multiaddr?active=active",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns multiple addresses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6bd07a59-3bdf-4a77-a553-d569277bf62f"
            }
          ]
        }
      ]
    }
  ]
}