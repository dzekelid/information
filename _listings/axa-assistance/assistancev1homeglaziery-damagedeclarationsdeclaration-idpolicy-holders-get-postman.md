{
  "info": {
    "name": "AXA Assistance Gets the information linked to the policy holder of the glaziery damage declaration",
    "_postman_id": "af4b31b7-5181-4fad-98da-de76e56d7ad6",
    "description": "Gets the information linked to the policy holder of the glaziery damage declaration",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "insurance",
      "item": [
        {
          "id": "84284ebf-e6d7-48aa-be77-dff26cc744a2",
          "name": "getAssistanceV1HomeGlaziery_damageDeclarationsDeclaration_idPolicy_holders",
          "request": {
            "url": {
              "protocol": "http",
              "host": "sandbox.api.axa-assistance.com",
              "path": [
                "assistance/v1/home/glaziery_damage/declarations/:declaration_id/policy_holders"
              ],
              "variable": [
                {
                  "id": "declaration_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the information linked to the policy holder of the glaziery damage declaration"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46742d5f-5def-40c8-998d-f22fd0cf0cac"
            }
          ]
        }
      ]
    }
  ]
}