{
  "info": {
    "name": "Lisk Requests multisignature membership data",
    "_postman_id": "d18dfde6-44c5-43d3-9474-6533f714b40c",
    "description": "Searches for the specified multisignature group and responds with a list of all members of this particular multisignature group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "98a096c9-c9e1-4650-8c90-7440e4b7b5c1",
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
              "id": "5660fe85-c1f1-44fc-a45a-1e8683c56654"
            }
          ]
        },
        {
          "id": "33f65e83-700f-4eee-8623-ec5bb1631451",
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
              "id": "06279fbe-8270-4b03-8114-efcabed44bbb"
            }
          ]
        },
        {
          "id": "4cddfa33-6925-418b-9940-5c40574b0515",
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
              "id": "c968f9b6-e248-4c19-aa1a-c40c7cb938c6"
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