{
  "info": {
    "name": "Blockchain Info Convert",
    "_postman_id": "11ce1443-73cd-4e84-9901-b0cbec521bd8",
    "description": "Convert x value in the provided currency to btc.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "0cce6e84-6c40-442b-b451-d7a40eb7c9b5",
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
              "id": "8fac02a3-679b-4bc8-94a0-4b8a5bda8082"
            }
          ]
        },
        {
          "id": "a5813409-b748-4d6c-8e72-49a0ef576900",
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
              "id": "57637d5d-685f-4cdd-9ab3-3cd4decc3d35"
            }
          ]
        }
      ]
    }
  ]
}