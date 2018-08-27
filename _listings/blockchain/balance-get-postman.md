{
  "info": {
    "name": "Blockchain Info Balance",
    "_postman_id": "76ad726f-9790-422d-8c93-58a62f7a6049",
    "description": "Returns current balance",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "4fb2ecfd-24f6-486d-bebc-939b35c816b9",
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
              "id": "5d2cec14-fb35-40f0-aa12-45b758eb185f"
            }
          ]
        },
        {
          "id": "bc4e8dd9-314a-48da-b2b3-aebb27d465e3",
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
              "id": "af1b087d-2186-4204-8cb8-45d8c6f73d58"
            }
          ]
        },
        {
          "id": "f951fd59-3803-4415-8463-e062002363b5",
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
              "id": "571f3abc-9cfb-43e1-9a45-02db6580d67b"
            }
          ]
        },
        {
          "id": "53c0fc47-98f0-4c8c-9a1e-db4bc0e5a144",
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
              "id": "088e72c3-dcc0-40e3-8ca3-cb324d72ad20"
            }
          ]
        },
        {
          "id": "45e4ea2f-3e93-4a1f-8714-d15b174c157c",
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
              "id": "d9458d87-d8b9-4ccd-b5b6-2bc43eca68fe"
            }
          ]
        },
        {
          "id": "351e323d-5876-492f-8559-537f506cc65f",
          "name": "getRawTransaction",
          "request": {
            "url": {
              "protocol": "http",
              "host": "blockchain.info",
              "path": [
                "rawtx/:tx_hash"
              ],
              "variable": [
                {
                  "id": "tx_hash",
                  "value": "tx_hash",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a raw trasaction."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "907cf012-40eb-44cb-995b-7dd207a23897"
            }
          ]
        },
        {
          "id": "00e6fb71-d252-4f4c-b60b-9c3739df7f75",
          "name": "getChartType",
          "request": {
            "url": "http://blockchain.info/Blockchain,s?chart-type=chart-type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns chart types."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2aea96f-2c2c-4e1b-8e6f-8ca200f96756"
            }
          ]
        },
        {
          "id": "55b63ff9-9e90-48d8-9ddf-d4238af95f80",
          "name": "getBlockHeight",
          "request": {
            "url": {
              "protocol": "http",
              "host": "blockchain.info",
              "path": [
                "block-height/:block_height"
              ],
              "variable": [
                {
                  "id": "block_height",
                  "value": "block_height",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the height of block."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a45aaa2c-c205-43b8-9a57-f6eca6c63b83"
            }
          ]
        },
        {
          "id": "99e5ee65-348d-4ee6-b60b-36574f9ecc16",
          "name": "getRawAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "blockchain.info",
              "path": [
                "rawaddr/:bitcoin_address"
              ],
              "variable": [
                {
                  "id": "bitcoin_address",
                  "value": "bitcoin_address",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a single blockchain address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9331b9a1-11f4-4ecc-968d-bdad718377ec"
            }
          ]
        },
        {
          "id": "8eb86fae-2bab-4425-ba04-87d2b5608317",
          "name": "getMultipleAddresses",
          "request": {
            "url": "http://blockchain.info/multiaddr?active=active",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns multiple addresses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1470036d-eef3-4596-993d-22730bcd656d"
            }
          ]
        },
        {
          "id": "c29849be-5321-4be8-b09b-11644887f637",
          "name": "getUnspentOutput",
          "request": {
            "url": "http://blockchain.info/unspent?active=active",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Unspent output."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78efa56f-6b4e-4fbb-98e6-de4f10cc5a05"
            }
          ]
        },
        {
          "id": "ed4defb8-9f54-4476-8538-65c08162b06f",
          "name": "getBalance",
          "request": {
            "url": "http://blockchain.info/balance",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns current balance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "500cb4bd-4219-4423-9f05-65a855708bed"
            }
          ]
        }
      ]
    }
  ]
}