{
  "info": {
    "name": "RipaEx Accounts Delegates Fee",
    "_postman_id": "4444c0fe-485a-4464-81f1-f7591162fb2a",
    "description": "Get the delegate fee of an account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "b2b1cf57-27c7-4366-9f0c-ad074d79a03c",
          "name": "accounts.getBalance",
          "request": {
            "url": "http://api.ripaex.io/api/accounts/getBalance?address=%7B%7D",
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
            "description": "Get the balance of an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a1235f2-278f-44f0-83db-5a44b2b5359c"
            }
          ]
        },
        {
          "id": "42f27f2d-5a4c-4847-8196-4a2527633052",
          "name": "accounts.getPublickey",
          "request": {
            "url": "http://api.ripaex.io/api/accounts/getPublickey?address=%7B%7D",
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
            "description": "Get the public key of an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7bbd7ca-e12c-44c5-a656-3891ed93449b"
            }
          ]
        },
        {
          "id": "f8c214b5-8198-4345-b9eb-4e0564fa9534",
          "name": "accounts.getDelegatesFee",
          "request": {
            "url": "http://api.ripaex.io/api/accounts/delegates/fee",
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
            "description": "Get the delegate fee of an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "322c60c2-5dfe-4771-a0b2-a310e6517543"
            }
          ]
        }
      ]
    }
  ]
}