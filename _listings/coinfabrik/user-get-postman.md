{
  "info": {
    "name": "CoinFabrik Show current user",
    "_postman_id": "3fd3af12-261c-4c3f-9792-71409fde61d2",
    "description": "Get current user’s public information. To get user’s email or private information, use permissions wallet:user:email and wallet:user:read.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "88de3bb0-bc1d-4b9f-a318-b825b7ba5ab2",
          "name": "get-any-users-public-information-with-their-id",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.coinbase.com",
              "path": [
                "v2",
                "users/:user_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Get any user’s public information with their ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f40c298f-9bdf-47fa-83c3-fd4924d05a53"
            }
          ]
        },
        {
          "id": "6abada4d-9925-468e-a6f0-38b19428076a",
          "name": "get-current-users-public-information-to-get-users-email-or-private-information-use-permissions-walle",
          "request": {
            "url": "http://api.coinbase.com/v2/user",
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
            "description": "Get current user’s public information. To get user’s email or private information, use permissions wallet:user:email and wallet:user:read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12b6561e-c21b-450b-af94-24755e2cb514"
            }
          ]
        }
      ]
    }
  ]
}