{
  "info": {
    "name": "Blockchain Info Unspent",
    "_postman_id": "07e92e72-7732-4295-ab06-1f9a9f7c91fa",
    "description": "Unspent output.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "b8739988-25a9-4934-a1cb-54d19db914b5",
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
              "id": "dea6c55d-170f-4ef2-b609-31effa01d698"
            }
          ]
        },
        {
          "id": "3e5a5bb2-8d61-4c7b-9005-4388cb30cbbe",
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
              "id": "75fa5a81-6fcb-4e5d-b963-3b4886a5ca28"
            }
          ]
        },
        {
          "id": "e83bee77-ff20-4543-9730-7fbbcd9eb637",
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
              "id": "0a29bc88-5238-4324-b1d3-a4efc370b218"
            }
          ]
        },
        {
          "id": "8821b8e4-5add-4e0d-b5f2-441cb39c4613",
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
              "id": "ae89c7c1-576d-4eba-a4ce-35ab5ea63330"
            }
          ]
        },
        {
          "id": "e001e85d-d14c-4368-992b-33b815bace4d",
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
              "id": "f62937fc-5e2e-49d4-8346-56940a8dd26a"
            }
          ]
        },
        {
          "id": "d1c9f659-4b51-43a8-bcc5-26ce3f1580e3",
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
              "id": "9866fb8e-3e70-4bf9-afa1-7e461e6129be"
            }
          ]
        },
        {
          "id": "a45ceaf3-afcb-4809-9cd2-8118b47952bd",
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
              "id": "3baa6742-1d84-4841-8fe7-bead8748a4fa"
            }
          ]
        },
        {
          "id": "40a916dd-7252-49e6-a164-cfbbd0c0ec67",
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
              "id": "9b37a88a-eadc-4bc3-89ca-4e7beeb96123"
            }
          ]
        },
        {
          "id": "874aad03-ab92-4914-9863-648825651f25",
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
              "id": "9fcdeafd-b210-427e-a8e8-bb4438a034ef"
            }
          ]
        },
        {
          "id": "40317940-fe1d-42f9-b679-01b8f0f69599",
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
              "id": "7e1639de-f758-491b-b014-0b5eef01a4d1"
            }
          ]
        },
        {
          "id": "4b090020-de28-435a-8334-bebfbbaa611f",
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
              "id": "8d366b5c-53e1-40e0-abc5-c9ba28b193ce"
            }
          ]
        }
      ]
    }
  ]
}