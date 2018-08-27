{
  "info": {
    "name": "Lisk Requests peers data",
    "_postman_id": "50cab656-ed88-4991-89d9-eae5f68eb65e",
    "description": "Search for specified peers.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "dbc9319e-2148-46a2-9835-7023ed4f6db1",
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
              "id": "fb7cbd2d-1185-466b-bc4a-b8751fcb0bde"
            }
          ]
        },
        {
          "id": "041c1973-9a41-4969-8060-a6d6816d24b9",
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
              "id": "69c5ee96-deb7-4566-9cff-df311439a0b1"
            }
          ]
        },
        {
          "id": "cba4041e-5f54-432d-af85-d54a1d6a7e9b",
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
              "id": "6639db7e-2bf7-4c19-8051-3a5ab556b5b2"
            }
          ]
        },
        {
          "id": "5273489e-6f67-498a-aaec-6e28a37d628c",
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
              "id": "81e8bf85-3e02-4d12-bdbe-c12ee83767e1"
            }
          ]
        },
        {
          "id": "d5c0b3e1-1d23-4433-9487-942b268a92e9",
          "name": "getPeers",
          "request": {
            "url": "{{default}}/peers?broadhash=%7B%7D&height=%7B%7D&httpPort=%7B%7D&ip=%7B%7D&limit=%7B%7D&offset=%7B%7D&os=%7B%7D&sort=%7B%7D&state=%7B%7D&version=%7B%7D&wsPort=%7B%7D",
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
            "description": "Search for specified peers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0681c05-0a83-4b27-91db-176579ac6cff"
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