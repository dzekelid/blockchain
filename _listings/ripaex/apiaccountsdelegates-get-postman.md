{
  "info": {
    "name": "RipaEx Accounts Delegates",
    "_postman_id": "91aef48c-5a9a-4527-9885-d206048c1035",
    "description": "Get the delegates of an account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "8e223de4-a169-46a2-8141-9be82cb586ce",
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
              "id": "3177d036-3590-41ec-9f89-bc80ec4ea77f"
            }
          ]
        },
        {
          "id": "7d004cd2-1a40-4dce-88fa-1f9e90cf0cbf",
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
              "id": "805fdd19-7125-46ba-b416-19f8a46ca760"
            }
          ]
        },
        {
          "id": "11945639-1f39-45a0-899e-485556cdc7cf",
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
              "id": "a3a173b9-f723-4312-be34-140a796bc4f7"
            }
          ]
        },
        {
          "id": "4f083f56-487f-4b0e-b428-7277ea587c61",
          "name": "accounts.getDelegates",
          "request": {
            "url": "http://api.ripaex.io/api/accounts/delegates?address=%7B%7D&limit=%7B%7D&offset=%7B%7D&orderBy=%7B%7D",
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
            "description": "Get the delegates of an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1749b83e-b570-4a89-99e5-d05f2c6222be"
            }
          ]
        }
      ]
    }
  ]
}