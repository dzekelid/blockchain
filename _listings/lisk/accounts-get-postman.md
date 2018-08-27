{
  "info": {
    "name": "Lisk Requests account data",
    "_postman_id": "0d97846b-a8ee-4aab-8c2c-82916a7df0f8",
    "description": "Search for matching accounts in the system.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "f3cd319f-9423-43df-8d6e-ccda21aaaadb",
          "name": "getAccounts",
          "request": {
            "url": "{{default}}/accounts?address=%7B%7D&limit=%7B%7D&offset=%7B%7D&publicKey=%7B%7D&secondPublicKey=%7B%7D&sort=%7B%7D&username=%7B%7D",
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
            "description": "Search for matching accounts in the system."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "269281cc-8eca-4a31-bee0-87dd92378c54"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/api"
    }
  ]
}