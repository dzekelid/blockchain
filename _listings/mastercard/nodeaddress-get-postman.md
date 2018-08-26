{
  "info": {
    "name": "Mastercard Get Node Address",
    "_postman_id": "364fcca7-5e66-4521-a677-99627f8d6c85",
    "description": "Information about a specific node may be retrieved by its address.\nThis is useful when navigating the network.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "151538ce-2dd4-4b4c-9f17-711e05324973",
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
              "id": "a750e83f-6125-496b-9a7d-7fae8568d969"
            }
          ]
        },
        {
          "id": "35784037-4a5e-412a-a9a8-6ddea9287f37",
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
              "id": "f8988f02-7aba-42ba-b2e8-485d1a89371d"
            }
          ]
        },
        {
          "id": "10dc680a-51f2-4263-9f9e-d6f8460aaa5c",
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
              "id": "32f34447-62ed-43f5-95c0-aa2029b60f9d"
            }
          ]
        }
      ]
    }
  ]
}