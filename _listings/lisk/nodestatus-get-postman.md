{
  "info": {
    "name": "Lisk Requests status data",
    "_postman_id": "2253108e-52bd-44ad-b1b1-269bfffc8ec7",
    "description": "Returns all current status data of the node, e.g. height and broadhash.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "e7a9cf88-399d-4115-b299-4fbc38c76fd0",
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
              "id": "497cb735-1cff-4455-9c43-fcf3068241c2"
            }
          ]
        },
        {
          "id": "8f99fe3e-8581-4700-b9fc-48b1a8bd3dca",
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
              "id": "81e788f1-52d1-4a0e-ac96-23b625a99bdf"
            }
          ]
        },
        {
          "id": "29e3f473-0c68-4a55-a0e0-0887b3130c28",
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
              "id": "0992b4c0-a8c0-45e1-9ba1-a0ab0f35c016"
            }
          ]
        },
        {
          "id": "68c06ec6-7db7-4560-b0d4-289ee84c63f7",
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
              "id": "09ff4907-1f62-458e-a959-5cc1fc89fe2f"
            }
          ]
        },
        {
          "id": "ab9c907c-f7a2-45db-9f2f-89b1cf8aa601",
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
              "id": "83124523-a6a4-427b-a743-5088a950101a"
            }
          ]
        },
        {
          "id": "7f4446ed-caea-459e-8855-a5ffdbed4f12",
          "name": "getConstants",
          "request": {
            "url": "{{default}}/node/constants",
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
            "description": "Returns all current constants data on the system, e.g. Lisk epoch time and version."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a76814f6-3720-43f1-8296-bd929dec2842"
            }
          ]
        },
        {
          "id": "1364765c-d2d9-478a-99d8-d39f9c60a93f",
          "name": "getStatus",
          "request": {
            "url": "{{default}}/node/status",
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
            "description": "Returns all current status data of the node, e.g. height and broadhash."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fdeeb4ec-b831-46bc-8c61-cf5bfc3ba7e8"
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