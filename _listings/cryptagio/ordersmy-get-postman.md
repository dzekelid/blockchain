{
  "info": {
    "name": "Cryptagio GetMy  Orders",
    "_postman_id": "989e47bc-0155-404b-952d-ddbc15c80282",
    "description": "Trades are sorted in reverse creation order.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "29448b8e-7177-4c11-8265-814e320ec88e",
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
              "id": "e1d57809-d5c0-4685-a5a6-357b786f9040"
            }
          ]
        },
        {
          "id": "cf6f48d0-012b-41ab-80ad-2b0352a367fe",
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
              "id": "2553fbc3-c38f-428f-b48c-25043897e5cd"
            }
          ]
        },
        {
          "id": "c34ecdcf-f1e3-4434-bec9-cc24cf70f8fd",
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
              "id": "a1dae31a-6e9e-4096-9f09-4fe184987c95"
            }
          ]
        },
        {
          "id": "36f46ac9-29f8-4a43-a7de-8acb492f7ab4",
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
              "id": "175aea7f-472d-4141-8bdb-803b59b8debf"
            }
          ]
        },
        {
          "id": "c916eeca-916c-4dbe-85a3-cf9a71d9e922",
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
              "id": "c8cbd817-9ac5-4555-b497-3fb9c89ca760"
            }
          ]
        },
        {
          "id": "98a2b1f8-eb4d-4f05-b596-7c1a54333aa3",
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
              "id": "029cce20-d9f1-4c88-ad38-24824eccba9c"
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