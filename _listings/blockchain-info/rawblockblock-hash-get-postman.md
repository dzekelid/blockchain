{
  "info": {
    "name": "Blockchain Info Raw Block",
    "_postman_id": "84bb752c-fdfa-4862-bf2c-59fac5eadfdd",
    "description": "Returns a single raw block.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "f546895d-79aa-44f6-b39e-1462647576f6",
          "name": "getTicker",
          "request": {
            "url": "http://blockchain.info/ticker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a JSON object with the currency codes as keys. \"15m\" is the 15 minutes delayed market price, \"last\" is the most recent market price, \"symbol\" is the currency symbol."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5426a853-7e23-48bc-9d82-15483dbf7158"
            }
          ]
        },
        {
          "id": "a875e7ad-d860-4613-9da1-a479a6c39a0f",
          "name": "convertToBTC",
          "request": {
            "url": "http://blockchain.info/tobtc?currency=currency&value=value",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Convert x value in the provided currency to btc."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a05302ac-702b-4a11-909c-896dd16c0e55"
            }
          ]
        },
        {
          "id": "9707430b-9548-407a-a0b0-139d4b22a14c",
          "name": "getStats",
          "request": {
            "url": "http://blockchain.info/stats?format=format",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This method can be used to get the data behind Blockchain.info's stats."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b033a247-8385-4375-a53b-6ef4dc2cefc1"
            }
          ]
        },
        {
          "id": "12b6edee-c35d-42d0-886a-7cef5d3b09f3",
          "name": "getPools",
          "request": {
            "url": "http://blockchain.info/pools?timespan=timespan",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This method can be used to get the data behind Blockchain.info's pools information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34175346-4e9e-4766-b3e5-000171ae9d2a"
            }
          ]
        },
        {
          "id": "f4793573-383d-4b14-890c-371eaa6b3615",
          "name": "getRawBlock",
          "request": {
            "url": {
              "protocol": "http",
              "host": "blockchain.info",
              "path": [
                "rawblock/:block_hash"
              ],
              "variable": [
                {
                  "id": "block_hash",
                  "value": "block_hash",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a single raw block."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9c53928-51b3-4f4a-b271-dbeaa46621e4"
            }
          ]
        }
      ]
    }
  ]
}