{
  "info": {
    "name": "Lisk Requests constants data",
    "_postman_id": "efd33d18-c48a-4b93-9f8a-94e7a58450e9",
    "description": "Returns all current constants data on the system, e.g. Lisk epoch time and version.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "557f6345-6274-436b-a57e-b7134d1061bf",
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
              "id": "515b38ff-d739-4fdc-b6a0-b9e8de4b26c1"
            }
          ]
        },
        {
          "id": "ea34b18b-eb86-4d55-be57-7199595fc2fc",
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
              "id": "a021854d-4f41-430d-827c-0c2b1aa16734"
            }
          ]
        },
        {
          "id": "f4bfbf9c-ae4c-42d9-b755-6d3b240d40d3",
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
              "id": "c375a4a2-2b59-45d7-82e5-49ab2f3b3f61"
            }
          ]
        },
        {
          "id": "2314f5d6-b06f-4255-b589-9f67f660bd18",
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
              "id": "a185266c-641b-4123-83bc-f4a1906725b0"
            }
          ]
        },
        {
          "id": "f01b6219-c7c9-41c6-82b8-a2e07331a70b",
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
              "id": "c8160d99-467e-470d-84e7-63454b8f8a05"
            }
          ]
        },
        {
          "id": "d602bfe7-a03d-49dc-b39b-baa4d09e7dfd",
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
              "id": "faaa536f-0884-4958-8503-e1f0261b2ea3"
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