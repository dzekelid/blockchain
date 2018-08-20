{
  "info": {
    "name": "Cryptagio Post Orders",
    "_postman_id": "87ad8324-38ad-420c-bea9-27cc557bf6e9",
    "description": "Accepts an array of JSON objects.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "ec80c149-9d30-4645-b11d-e7333b24cc75",
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
              "id": "693c7d17-a18a-4ad0-be0e-0fa53300dbc4"
            }
          ]
        },
        {
          "id": "91ffb6e0-cc47-41c0-8ecd-b4d7b1dcf080",
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
              "id": "20550f87-ad1b-4c57-b434-2ef72040ffe1"
            }
          ]
        },
        {
          "id": "7c975b2b-bfaa-4c3c-8142-16448989c01c",
          "name": "getTrades",
          "request": {
            "url": "{{default}}/trades?from_time=%7B%7D&from_uuid=%7B%7D&limit=%7B%7D&market=%7B%7D&order=%7B%7D&side=%7B%7D&to_time=%7B%7D",
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
            "description": "Get recent trades on market, each trade is included only once. Trades are sorted in reverse creation order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8af5acdb-7f91-438a-8c34-b31154d99137"
            }
          ]
        },
        {
          "id": "90431980-d633-4450-9e9f-ef3a42f856cc",
          "name": "getTradesMy",
          "request": {
            "url": "{{default}}/trades/my?from_time=%7B%7D&from_uuid=%7B%7D&limit=%7B%7D&market=%7B%7D&order=%7B%7D&side=%7B%7D&to_time=%7B%7D",
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
            "description": "Trades are sorted in reverse creation order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9c9865a-5df6-47c7-936c-7db40ce03a81"
            }
          ]
        },
        {
          "id": "6b70ed97-48a2-42cd-ae01-80bd9847107a",
          "name": "getBalances",
          "request": {
            "url": "{{default}}/balances",
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
            "description": "Get user balances.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa53164d-da12-461b-9b9e-e65c607b01f1"
            }
          ]
        },
        {
          "id": "4e4c3550-f6f8-4635-9e62-fc0ed8494d45",
          "name": "getOrdersMy",
          "request": {
            "url": "{{default}}/orders/my?from_time=%7B%7D&from_uuid=%7B%7D&limit=%7B%7D&market=%7B%7D&order=%7B%7D&side=%7B%7D&status=%7B%7D&to_time=%7B%7D&type=%7B%7D",
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
            "description": "Trades are sorted in reverse creation order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6bf8fc01-d54b-4614-b226-f0584e58e8e8"
            }
          ]
        },
        {
          "id": "552cf271-cb10-4c25-b87c-c9b1fcfb65f4",
          "name": "postOrders",
          "request": {
            "url": "{{default}}/orders",
            "method": "POST",
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
            "description": "Accepts an array of JSON objects."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "432493a8-7854-4b52-9251-a43c51c9c71b"
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