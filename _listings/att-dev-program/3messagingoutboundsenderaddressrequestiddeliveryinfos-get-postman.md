{
  "info": {
    "name": "AT&T API Get Messaging Outbound Senderaddress Requestid Deliveryinfos",
    "_postman_id": "b9e3e7c1-7b73-41d6-93fb-6d070a7e8e74",
    "description": "/3/messaging/outbound/{senderAddress}/{requestId}/deliveryInfos",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Devicecapabilities",
      "item": [
        {
          "id": "8cdbc8da-c74a-44c1-b92d-0a8f8b4e5f34",
          "name": "1devicecapabilitiesacrauthorizationcapabilities",
          "request": {
            "url": "http://api.att.com/1/devicecapabilities/acr:authorization/capabilities",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/1/devicecapabilities/acr:authorization/capabilities"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29070cf3-b429-4893-a603-745ca68bc3e4"
            }
          ]
        }
      ]
    },
    {
      "name": "Messaging",
      "item": [
        {
          "id": "768cdbab-8c8b-4527-a18c-7d4b3e4124ae",
          "name": "3messagingoutboundsenderaddressrequests",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.att.com",
              "path": [
                "3/messaging/outbound/:senderAddress/requests"
              ],
              "variable": [
                {
                  "id": "senderAddress",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/3/messaging/outbound/{senderAddress}/requests"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5350d97f-058e-4b96-b7fe-0c20ddd77987"
            }
          ]
        },
        {
          "id": "680d47b9-c147-4e22-bd41-eeeafa31a48e",
          "name": "3messagingoutboundsenderaddressrequestiddeliveryinfos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.att.com",
              "path": [
                "3/messaging/outbound/:senderAddress/:requestId/deliveryInfos"
              ],
              "variable": [
                {
                  "id": "requestId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "senderAddress",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/3/messaging/outbound/{senderAddress}/{requestId}/deliveryInfos"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "edeec14a-5697-41c5-8e24-ccb02c50e0ca"
            }
          ]
        }
      ]
    }
  ]
}