{
  "info": {
    "name": "CoinFabrik Show a user",
    "_postman_id": "37e4f68e-e3ee-4839-822a-46e3bbf5c398",
    "description": "Get any user’s public information with their ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "8e7c55c4-96b6-45c5-900c-86c501720e97",
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
              "id": "5e01bb67-7592-4b56-8740-4b8660c9d315"
            }
          ]
        }
      ]
    }
  ]
}