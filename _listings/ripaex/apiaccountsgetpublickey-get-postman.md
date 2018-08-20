{
  "info": {
    "name": "RipaEx Accounts Get Publickey",
    "_postman_id": "0f4faba4-46ce-4741-a658-451db456fd0c",
    "description": "Get the public key of an account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "806c351f-ea80-4dcd-a97e-9106a799ad03",
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
              "id": "f23cf606-9d5b-4903-8f18-dea2f46b7970"
            }
          ]
        },
        {
          "id": "38c3e2fd-3fe6-4368-83e6-6a985b0b7af1",
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
              "id": "46503876-5550-4de7-bd31-662fb239ed65"
            }
          ]
        }
      ]
    }
  ]
}