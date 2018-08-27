{
  "info": {
    "name": "Crypto Compare Get Multiple Prices",
    "_postman_id": "42cf7d01-dc6a-4c05-b321-3321185b9454",
    "description": "Get multiple prices.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Discovery",
      "item": [
        {
          "id": "b0118383-220b-456b-a664-4ee4b78337e3",
          "name": "UnnammedEndpointGet",
          "request": {
            "url": "http://min-api.cryptocompare.com/",
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
            "description": "Api description."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3509d5a5-e8eb-41f3-978e-48500b2a1f2b"
            }
          ]
        }
      ]
    },
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "a2e9f8ee-2355-41fe-b705-44ed27cc3d13",
          "name": "DataPriceGet",
          "request": {
            "url": "http://min-api.cryptocompare.com/data/price?fsym=%7B%7D&tsyms=%7B%7D",
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
            "description": "Get single price."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c8b8f41-3b70-4876-b737-e73a5c2a8446"
            }
          ]
        },
        {
          "id": "3aae393e-a1c4-43af-911f-0fe240363a22",
          "name": "DataPricemultiGet",
          "request": {
            "url": "http://min-api.cryptocompare.com/data/pricemulti?fsyms=%7B%7D&tsyms=%7B%7D",
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
            "description": "Get multiple prices."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f36c38fe-96a3-4a95-ad24-63a48d69398c"
            }
          ]
        }
      ]
    }
  ]
}