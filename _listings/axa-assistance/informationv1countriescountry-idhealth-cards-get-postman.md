{
  "info": {
    "name": "AXA Assistance Retrieve health information for a country",
    "_postman_id": "e01b2c1c-312b-4229-a4bf-242c41371bb5",
    "description": "Retrieve health information for a country",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "insurance",
      "item": [
        {
          "id": "fe85b986-8e68-488c-984b-18eb6a2372db",
          "name": "getInformationV1CountriesCountry_idHealth_cards",
          "request": {
            "url": {
              "protocol": "http",
              "host": "sandbox.api.axa-assistance.com",
              "path": [
                "information/v1/countries/:country_id/health_cards"
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
            "description": "Retrieve health information for a country"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c525f855-ee0f-4a59-b092-2a1182408298"
            }
          ]
        }
      ]
    }
  ]
}