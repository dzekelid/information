{
  "info": {
    "name": "Plentymarkets Get legal information of an online store",
    "_postman_id": "ec5e1c8d-fc41-4cce-b49e-96701f851826",
    "description": "Gets legal information of an online store. The plenty ID of the store , the language and the type of legal information must be specified. The language must be specified as ISO 639-1 code.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Legal",
      "item": [
        {
          "id": "01bcc8f0-6975-4a29-bf8f-43cd8d2ce680",
          "name": "getRestLegalinformationPlentyLangType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/legalinformation/:plentyId/:lang/:type"
              ],
              "variable": [
                {
                  "id": "lang",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "plentyId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "type",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Gets legal information of an online store. The plenty ID of the store , the language and the type of legal information must be specified. The language must be specified as ISO 639-1 code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ec913ee-81a5-48ba-93ff-8d93d2ab89f3"
            }
          ]
        }
      ]
    }
  ]
}