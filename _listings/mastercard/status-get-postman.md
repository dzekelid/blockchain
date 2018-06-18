{
  "info": {
    "name": "Mastercard Get Status",
    "_postman_id": "674f324a-aa2c-4a7f-9814-c1ae609c1c77",
    "description": "Gets general metadata about the current state of the blockchain network.\nUseful for building dashboards.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "a781f286-56b3-477f-911c-02f29bca916a",
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
              "id": "9a2a7807-65a3-4133-8d86-f5c3fc0784fb"
            }
          ]
        }
      ]
    }
  ]
}