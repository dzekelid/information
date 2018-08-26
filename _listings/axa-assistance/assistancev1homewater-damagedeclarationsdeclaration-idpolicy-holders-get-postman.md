{
  "info": {
    "name": "AXA Assistance Gets the information related to each the policy holder of the water damage declaration",
    "_postman_id": "965c9acc-1d01-4895-aaf4-6e29897314a9",
    "description": "Gets the information related to each the policy holder of the water damage declaration",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "insurance",
      "item": [
        {
          "id": "2ad532b8-c3bd-4c08-87c1-803a8f5a5695",
          "name": "getAssistanceV1HomeWater_damageDeclarationsDeclaration_idPolicy_holders",
          "request": {
            "url": {
              "protocol": "http",
              "host": "sandbox.api.axa-assistance.com",
              "path": [
                "assistance/v1/home/water_damage/declarations/:declaration_id/policy_holders"
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
            "description": "Gets the information related to each the policy holder of the water damage declaration"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fef90ff8-3aee-47be-969d-14b40ed72349"
            }
          ]
        }
      ]
    }
  ]
}