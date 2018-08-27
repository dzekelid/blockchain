{
  "info": {
    "name": "Lisk Requests dapps data",
    "_postman_id": "0b736924-d29a-41f1-bf3c-a9efa2057287",
    "description": "Search for a specified dapp in the system.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "f1c8158e-d53c-4c68-b61e-a74dfd374205",
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
              "id": "c7de372c-70fd-4089-b024-78fdc6a62356"
            }
          ]
        },
        {
          "id": "d310392d-3403-4576-bf3b-bb7bbbdf8c5c",
          "name": "getMultisignatureGroups",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:address/multisignature_groups"
              ],
              "variable": [
                {
                  "id": "address",
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
            "description": "Searches for the specified account in the system and responds with a list of the multisignature groups that this account is member of."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38c839eb-891d-4c92-ae3e-ff80004d06bf"
            }
          ]
        },
        {
          "id": "9526d637-fa16-4665-9aac-eb736307a8e8",
          "name": "getMultisignatureMemberships",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:address/multisignature_memberships"
              ],
              "variable": [
                {
                  "id": "address",
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
            "description": "Searches for the specified multisignature group and responds with a list of all members of this particular multisignature group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61aa766f-2aca-4422-acfe-1fb302e80bb9"
            }
          ]
        },
        {
          "id": "a99d9862-017c-4f0e-a5eb-818f4df520cb",
          "name": "getDapps",
          "request": {
            "url": "{{default}}/dapps?limit=%7B%7D&name=%7B%7D&offset=%7B%7D&sort=%7B%7D&transactionId=%7B%7D",
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
            "description": "Search for a specified dapp in the system."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b734182-4b93-4e0b-b05e-05688ab36d4b"
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