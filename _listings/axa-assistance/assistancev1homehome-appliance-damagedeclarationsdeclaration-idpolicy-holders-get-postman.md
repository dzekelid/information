{
  "info": {
    "name": "AXA Assistance Gets the information linked to the policy holder of the home appliance damage declaration",
    "_postman_id": "660a8d00-760a-4be7-806f-c05c1650a9f1",
    "description": "Gets the information linked to the policy holder of the home appliance damage declaration",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "insurance",
      "item": [
        {
          "id": "b0df0707-9005-4f09-b3e2-35dc1da8ebbb",
          "name": "getAssistanceV1HomeHome_appliance_damageDeclarationsDeclaration_idPolicy_holders",
          "request": {
            "url": {
              "protocol": "http",
              "host": "sandbox.api.axa-assistance.com",
              "path": [
                "assistance/v1/home/home_appliance_damage/declarations/:declaration_id/policy_holders"
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
            "description": "Gets the information linked to the policy holder of the home appliance damage declaration"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "240b7663-e356-4445-bb63-b3dac7e1ec6a"
            }
          ]
        }
      ]
    }
  ]
}