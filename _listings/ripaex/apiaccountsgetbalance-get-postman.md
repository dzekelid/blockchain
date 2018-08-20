{
  "info": {
    "name": "RipaEx Accounts Get Balance",
    "_postman_id": "51f9a5bf-5798-4068-af56-570189dde8e5",
    "description": "Get the balance of an account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "7105aed5-f457-480d-b542-f2173c088800",
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
              "id": "55a037d9-4290-41db-b2b1-b943799f4fba"
            }
          ]
        }
      ]
    }
  ]
}