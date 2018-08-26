{
  "info": {
    "name": "AXA Assistance Retrieve security information for a country",
    "_postman_id": "2ef6cf6d-c911-484d-9192-8c9f6975da29",
    "description": "Retrieve security information for a country",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "insurance",
      "item": [
        {
          "id": "ba34cef3-29cd-459f-b5e2-a57dae44bcc6",
          "name": "getInformationV1CountriesCountry_idSecurity_cards",
          "request": {
            "url": {
              "protocol": "http",
              "host": "sandbox.api.axa-assistance.com",
              "path": [
                "information/v1/countries/:country_id/security_cards"
              ],
              "variable": [
                {
                  "id": "country_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "accept-language",
                "value": "{}",
                "description": "Language/Country",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve security information for a country"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1dd4f248-c2f7-4112-8dae-e4cd0788f3f1"
            }
          ]
        }
      ]
    }
  ]
}