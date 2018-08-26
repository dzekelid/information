{
  "info": {
    "name": "AXA Assistance Gets assignment information.",
    "_postman_id": "07c10346-602f-43da-97ff-df85cafba99d",
    "description": "Gets assignment information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "insurance",
      "item": [
        {
          "id": "40af3c35-8588-4f43-9f17-c4e3b4f08c49",
          "name": "getServiceVexpRoadsideAssignmentsAssignment_id",
          "request": {
            "url": {
              "protocol": "http",
              "host": "sandbox.api.axa-assistance.com",
              "path": [
                "service/vexp/roadside/assignments/:assignment_id"
              ],
              "variable": [
                {
                  "id": "assignment_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets assignment information"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0c6e269-2dee-411b-9ab0-11f66eabcf94"
            }
          ]
        }
      ]
    }
  ]
}