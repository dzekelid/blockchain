{
  "info": {
    "name": "Blockchain Info Block Height",
    "_postman_id": "b58cd14f-e9af-4127-8ba7-200b07e909ca",
    "description": "Returns the height of block.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "a6ebad1a-105a-4496-9187-5043a622c0a9",
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
              "id": "83836a3e-205c-4240-9d06-1d3243d00a89"
            }
          ]
        },
        {
          "id": "8405902e-5925-4164-9191-d8fa38b2d659",
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
              "id": "46db8399-c1f6-4c7b-9a02-4b1def5f9877"
            }
          ]
        },
        {
          "id": "a4ae09c5-772b-41be-aac5-ece107d8654d",
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
              "id": "64f08785-5a0e-4b3f-8365-a6d57a727b68"
            }
          ]
        },
        {
          "id": "3f91956d-6fe5-477c-9a53-8efbb41afb8c",
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
              "id": "88a48f12-848e-4c83-b5b2-cb7f352ffdad"
            }
          ]
        },
        {
          "id": "5e397bd7-88ac-418c-bb06-933f5199395e",
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
              "id": "5342cf6e-6dd4-469e-9071-71b6940d14de"
            }
          ]
        },
        {
          "id": "d708933e-9cd2-4154-9ae7-663075827987",
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
              "id": "89dec678-5552-42a1-9d9a-9a039150792e"
            }
          ]
        },
        {
          "id": "afd88962-f52b-411c-922b-65335d1b891c",
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
              "id": "be24d32b-42fb-4bb9-bea3-2b83572e0b05"
            }
          ]
        },
        {
          "id": "5521f38f-674b-4c96-aa16-85a7fc145663",
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
              "id": "19d342d6-4fce-4894-ad0c-155be6a11bd4"
            }
          ]
        }
      ]
    }
  ]
}