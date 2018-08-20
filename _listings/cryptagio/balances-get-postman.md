{
  "info": {
    "name": "Cryptagio Get Balances",
    "_postman_id": "a9ce7074-bf2b-46ac-9db8-fa54aa56a489",
    "description": "Get user balances..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "f43b5d6c-0ee4-49d1-a90b-f7ddf0f624d0",
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
              "id": "7dc300cc-39e9-474e-b0ba-a57f9d28b84f"
            }
          ]
        },
        {
          "id": "21e8df71-d00f-4ae5-8f33-1c49dedec99b",
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
              "id": "90bc989a-8b65-452b-9b94-c97fad594a02"
            }
          ]
        },
        {
          "id": "63b4232d-385e-465e-b8ed-e626e8da5b11",
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
              "id": "8b8deae0-0028-4379-bb9f-b30609145a87"
            }
          ]
        },
        {
          "id": "533c98e0-9128-4cd2-bf6d-332745c6eaee",
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
              "id": "75aeabf0-eea0-497b-8162-866aac6e3e23"
            }
          ]
        },
        {
          "id": "093626be-0bbd-49b2-8153-817268bea000",
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
              "id": "d54dc138-74c5-46db-b31e-30557c5aae9f"
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