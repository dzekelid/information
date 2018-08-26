{
  "info": {
    "name": "AXA Assistance Gets the information linked to the policy holder of the locksmithing damage declaration",
    "_postman_id": "ea3fff6f-6dba-4b4a-b08e-c4e8f0ea32c1",
    "description": "Gets the information linked to the policy holder of the locksmithing damage declaration",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "insurance",
      "item": [
        {
          "id": "e72419ed-6f23-43b5-a7da-3512b093690a",
          "name": "getAssistanceV1HomeLocksmithing_damageDeclarationsDeclaration_idPolicy_holders",
          "request": {
            "url": {
              "protocol": "http",
              "host": "sandbox.api.axa-assistance.com",
              "path": [
                "assistance/v1/home/locksmithing_damage/declarations/:declaration_id/policy_holders"
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
            "description": "Gets the information linked to the policy holder of the locksmithing damage declaration"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "efafb708-8663-4a6f-a8e7-9965b75e9537"
            }
          ]
        }
      ]
    }
  ]
}