{
  "info": {
    "name": "Blockchain Info Blocks for One Day",
    "_postman_id": "a9a2ec8a-e4e4-403a-b704-2ec329123c85",
    "description": "Returns the blocks for one day by the millisecond",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "a9c9a611-67a9-4df2-a759-3e77759a10ae",
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
              "id": "5af9ccba-cc42-49af-b591-31476eb64752"
            }
          ]
        },
        {
          "id": "ffb691ac-a3fb-4ce0-aedc-0b1eb1b4e632",
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
              "id": "3e1c3947-24ba-4fdf-b7bb-bcd7526cad4b"
            }
          ]
        },
        {
          "id": "3b24bb52-ebac-468d-bc73-596b95d86014",
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
              "id": "8c225a70-da08-43a1-8f3e-2a6e87e70105"
            }
          ]
        },
        {
          "id": "22dcec36-1b00-44a7-916f-6649372c1d83",
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
              "id": "d8efb498-bc93-45d9-862b-58c0b2817509"
            }
          ]
        },
        {
          "id": "933416e6-cce7-424d-98ee-5407a7c1094f",
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
              "id": "788e6965-efff-47da-b805-7f5b56a4c583"
            }
          ]
        },
        {
          "id": "9c194449-3e53-47e2-a4fc-b90a39dcb10e",
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
              "id": "d65cc756-b029-46c3-b206-ac17166dfea3"
            }
          ]
        },
        {
          "id": "1270773b-cf50-4366-9895-a6d07ef514f8",
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
              "id": "4d4755bd-4132-48f4-b45c-8072c3df5c41"
            }
          ]
        },
        {
          "id": "168a2c14-7efc-4714-8a65-43c031db8245",
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
              "id": "41a3df53-b888-417b-9c4e-33606c4b5ac3"
            }
          ]
        },
        {
          "id": "6658d3f6-0ff3-45d3-986f-20fd1c4a55ba",
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
              "id": "85b0b7e7-d8dc-449e-a8ce-218da1fb5acb"
            }
          ]
        },
        {
          "id": "48ca75eb-5396-4a7d-a4a6-fb2ca70df949",
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
              "id": "4ef636f7-8d4a-4a54-b402-aedafe223a47"
            }
          ]
        },
        {
          "id": "52fcdeee-3bfc-4675-81b8-5b2b3777e652",
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
              "id": "11e9645c-bc18-4ddb-94a4-d4cf8e78b7ce"
            }
          ]
        },
        {
          "id": "df20daa2-3b96-4f22-8361-b02070c66762",
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
              "id": "a82f751d-3e3e-421c-be4a-ddc5bc41a5a3"
            }
          ]
        },
        {
          "id": "a46e82dd-0178-4716-b642-b757efa1c403",
          "name": "getLatestBlock",
          "request": {
            "url": "http://blockchain.info/latestblock?format=format",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the latest block."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59f5f550-8fbf-4f6c-9255-c07c93b8b3ec"
            }
          ]
        },
        {
          "id": "86a82625-2b79-48ce-867c-1ea50fcbbf6a",
          "name": "getUnconfirmedTransactions",
          "request": {
            "url": "http://blockchain.info/unconfirmed-transactions",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns unconfirmed transactions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc3cbd10-ba8c-4de1-bfc0-0a24671cc135"
            }
          ]
        },
        {
          "id": "29f205e7-ddba-44d8-8342-fb60de87247b",
          "name": "getBlocksOneDay",
          "request": {
            "url": {
              "protocol": "http",
              "host": "blockchain.info",
              "path": [
                "blocks/:time_in_milliseconds"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "time_in_milliseconds",
                  "value": "time_in_milliseconds",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the blocks for one day by the millisecond"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81d7f0c1-cf5c-4bbe-ac5a-ba754b9df02e"
            }
          ]
        }
      ]
    }
  ]
}