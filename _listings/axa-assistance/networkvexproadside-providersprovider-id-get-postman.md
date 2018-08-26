{
  "info": {
    "name": "AXA Assistance Gets information of roadside provider.",
    "_postman_id": "fe38be60-01fc-4ea7-8ed2-20ce4533acbf",
    "description": "Gets information of roadside provider.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "insurance",
      "item": [
        {
          "id": "af3e1443-f029-4b7c-ab51-a1796ef638cc",
          "name": "getNetworkVexpRoadside_providersProvider_id",
          "request": {
            "url": {
              "protocol": "http",
              "host": "sandbox.api.axa-assistance.com",
              "path": [
                "network/vexp/roadside_providers/:provider_id"
              ],
              "variable": [
                {
                  "id": "provider_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information of roadside provider"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4bf1616a-ea56-473e-a7ae-10c2466850eb"
            }
          ]
        }
      ]
    }
  ]
}