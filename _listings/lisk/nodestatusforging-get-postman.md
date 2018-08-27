{
  "info": {
    "name": "Lisk Requests forging status of a delegate",
    "_postman_id": "fb5683a6-b1dc-4a9a-960f-08a82ae3326f",
    "description": "*Attention! This is a **private endpoint only authorized to whitelisted IPs.**\nTo edit the whitelist, please edit the `forging.access.whitelist` section in `config.json`*<br>\nResponds with the forging status of a delegate on a node.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "6d482d37-d3c4-4175-935b-7c256a7f4301",
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
              "id": "f9ec3556-18b9-439c-a3b9-3a75607fe248"
            }
          ]
        },
        {
          "id": "60776ddc-227d-40fa-8b19-ea1628fcf0f1",
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
              "id": "14a8fec0-f50b-4625-8bcc-0e4aa08fe13a"
            }
          ]
        },
        {
          "id": "db76af92-0732-491f-8f82-bd0c313b672a",
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
              "id": "786f9251-3152-4172-b9ea-caf283544c1e"
            }
          ]
        },
        {
          "id": "f189de4a-9ec1-40a7-a0e1-34cf9419f6c9",
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
              "id": "dbb8ffc0-0c0a-44a6-92ae-a775e34641e2"
            }
          ]
        },
        {
          "id": "50a48413-f8f8-4d47-a58d-1a0d08345d1d",
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
              "id": "11978ec9-a421-4988-8f59-bab956a374ab"
            }
          ]
        },
        {
          "id": "73baf77e-bc9b-4267-9d44-652c29aaa656",
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
              "id": "e270ff63-fda9-4127-b118-22f9821306a4"
            }
          ]
        },
        {
          "id": "09c579e0-1b96-495f-b19a-27f062f5113d",
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
              "id": "64f2fbda-2f89-4816-89c0-730ba287d5a0"
            }
          ]
        },
        {
          "id": "8c151987-4fe0-4624-b5c0-a5989699c317",
          "name": "getForgingStatus",
          "request": {
            "url": "{{default}}/node/status/forging?publicKey=%7B%7D",
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
            "description": "*Attention! This is a **private endpoint only authorized to whitelisted IPs.**\nTo edit the whitelist, please edit the `forging.access.whitelist` section in `config.json`*<br>\nResponds with the forging status of a delegate on a node."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5704505b-9c00-4eed-8615-b6c19a3d11c5"
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