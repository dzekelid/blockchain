{
  "info": {
    "name": "Mastercard Get Node",
    "_postman_id": "3db3e1bf-8601-4323-b77b-1d69e442b040",
    "description": "By default, this call gets information about your local node and its\nconnections. The `scope` parameter enabled this query to be extended\nto get further information about nodes that are visible to your node.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "a0106eab-c413-4e73-9c9f-b4ecd8d16e50",
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
              "id": "6dec7676-139f-45e9-b9ac-241d7bbbc9b5"
            }
          ]
        },
        {
          "id": "7c21e5fe-77a2-4fc4-88c6-e8ae2cffec90",
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
              "id": "602fcd54-30f4-41e5-898f-73060ff6519d"
            }
          ]
        }
      ]
    }
  ]
}