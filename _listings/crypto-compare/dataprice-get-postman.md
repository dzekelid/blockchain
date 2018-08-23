{
  "info": {
    "name": "Crypto Compare Get Single Price",
    "_postman_id": "df730d3f-601b-45ae-a602-f08c5530b1cf",
    "description": "Get single price.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Discovery",
      "item": [
        {
          "id": "c543f689-696d-4cd4-a7b3-7f2f8c6cb6d9",
          "name": "UnnammedEndpointGet",
          "request": {
            "url": "http://min-api.cryptocompare.com/",
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
            "description": "Api description."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32375f3a-e977-429e-af8b-5c2b783189f7"
            }
          ]
        }
      ]
    },
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "9423df77-cda4-47ae-90e8-31435f3e3e71",
          "name": "DataPriceGet",
          "request": {
            "url": "http://min-api.cryptocompare.com/data/price?fsym=%7B%7D&tsyms=%7B%7D",
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
            "description": "Get single price."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0385eb8-061a-4097-8255-5e2dee33ced1"
            }
          ]
        }
      ]
    }
  ]
}