{
  "info": {
    "name": "Mastercard Get App",
    "_postman_id": "4a2bbf6c-88a5-48cd-8a75-da59681fda92",
    "description": "Information about an application referenced by the `id` parameter. If\nyou are permissioned to that application, this will also return the\nmessage definitions you will need to comply with to issue valid transaction\nentries for that application.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "ad1baf12-ca0e-49f4-b113-4a2b3f4dddc3",
          "name": "getStatus",
          "request": {
            "url": "http://eas5stl0.mastercard.int:13046/z0/core/v1/status",
            "method": "GET",
            "header": [
              {
                "key": "MCWSSAML",
                "value": "{}",
                "description": "SAML Authorization",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets general metadata about the current state of the blockchain network.\nUseful for building dashboards."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88246bc4-b189-47ac-b53e-1ea52826d09e"
            }
          ]
        },
        {
          "id": "01c6fd96-cbba-4e91-ab20-a576b0031522",
          "name": "getNode",
          "request": {
            "url": "http://eas5stl0.mastercard.int:13046/z0/core/v1/node?scope=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "MCWSSAML",
                "value": "{}",
                "description": "SAML Authorization",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "By default, this call gets information about your local node and its\nconnections. The `scope` parameter enabled this query to be extended\nto get further information about nodes that are visible to your node."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7fee9b4e-eb65-4a2d-b845-e66def68b968"
            }
          ]
        },
        {
          "id": "c3d587d2-b74c-46c3-ae80-ed4d5f338d0c",
          "name": "getNodeAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "eas5stl0.mastercard.int",
              "path": [
                "z0",
                "core",
                "v1",
                "node/:address"
              ],
              "port": "13046",
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
                "key": "MCWSSAML",
                "value": "{}",
                "description": "SAML Authorization",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Information about a specific node may be retrieved by its address.\nThis is useful when navigating the network."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7bc6411b-32ad-476c-9793-7677540cbc21"
            }
          ]
        },
        {
          "id": "20ced81d-fda7-488b-93d7-12a535c6b032",
          "name": "getApp",
          "request": {
            "url": {
              "protocol": "http",
              "host": "eas5stl0.mastercard.int",
              "path": [
                "z0",
                "core",
                "v1",
                "app/:id"
              ],
              "port": "13046",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "MCWSSAML",
                "value": "{}",
                "description": "SAML Authorization",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Information about an application referenced by the `id` parameter. If\nyou are permissioned to that application, this will also return the\nmessage definitions you will need to comply with to issue valid transaction\nentries for that application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b299798-6820-4dfd-8e22-6ff0c54fe8c4"
            }
          ]
        }
      ]
    }
  ]
}