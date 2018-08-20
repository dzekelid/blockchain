{
  "info": {
    "name": "Cryptagio Post Orders Cancel",
    "_postman_id": "c67497bf-f2c5-46d6-a84e-9e7d3d05e18d",
    "description": "Accepts JSON object. Cancels all orders if no parameters are passed.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "ecc5828e-f570-41ce-a5c6-15e722cbaa58",
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
              "id": "6ea85c52-c986-4f47-876a-71c008004fe3"
            }
          ]
        },
        {
          "id": "f91529c3-2e79-4696-bd79-50fc37e46d3e",
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
              "id": "053f500a-bbdb-46da-b7f7-c92011928ef0"
            }
          ]
        },
        {
          "id": "3348b324-de38-4da4-ad06-a25df4103dd8",
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
              "id": "9afe5b99-0bbb-487e-a4fb-b47a5df6da5b"
            }
          ]
        },
        {
          "id": "36f56468-0382-4505-88e1-5b6d02ea9b57",
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
              "id": "938b3ce3-f3e2-4a5b-ae55-1cb3aaca89cf"
            }
          ]
        },
        {
          "id": "68977bd8-aade-4be7-9f38-0f8ca4c0c1db",
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
              "id": "87dad641-30c7-4a9f-9d2b-42b2e45fe8fb"
            }
          ]
        },
        {
          "id": "62e7e773-ae9b-47f6-9296-39baec6ebf91",
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
              "id": "40d5057d-0160-4b20-bad9-2dec4807382d"
            }
          ]
        },
        {
          "id": "4ad1260d-fb88-4101-9ab2-ff611b4d91e6",
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
              "id": "e891e91d-3e6f-463c-8312-22a722abc9f1"
            }
          ]
        },
        {
          "id": "883ce9e9-0970-48a8-89e3-6358398c1ba1",
          "name": "postOrdersCancel",
          "request": {
            "url": "{{default}}/orders/cancel",
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
            "description": "Accepts JSON object. Cancels all orders if no parameters are passed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6dad1da2-160e-4e5a-aa9f-f92122deb4a2"
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