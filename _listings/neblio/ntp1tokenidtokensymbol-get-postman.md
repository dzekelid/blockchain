{
  "info": {
    "name": "Neblio Returns the tokenId representing a token",
    "_postman_id": "cd24a148-0b4f-4883-b45e-79d36fe670b5",
    "description": "Translates a token symbol to a tokenId if a token exists with that symbol on the network",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "215ccf35-6597-4540-b66e-45c48cba36bc",
          "name": "getTokenId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "ntp1node.nebl.io",
              "path": [
                "ntp1/tokenid/:tokensymbol"
              ],
              "variable": [
                {
                  "id": "tokensymbol",
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
            "description": "Translates a token symbol to a tokenId if a token exists with that symbol on the network"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6826e96b-8147-401e-b184-1d3be3661c69"
            }
          ]
        }
      ]
    }
  ]
}