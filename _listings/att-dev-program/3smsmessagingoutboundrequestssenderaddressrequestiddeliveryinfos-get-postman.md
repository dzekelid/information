{
  "info": {
    "name": "AT&T API Get SMS Outbound Requests Senderaddress Requestid Deliveryinfos",
    "_postman_id": "04b9caeb-234f-4718-ab96-b7ed8ce2eec7",
    "description": "/3/smsmessaging/outbound/requests/{senderAddress}/{requestId}/deliveryInfos",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Devicecapabilities",
      "item": [
        {
          "id": "a95664bd-ce35-4e2a-8a9d-6b05afe02ab3",
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
              "id": "234e8fe5-1299-4731-8395-ee596a829699"
            }
          ]
        }
      ]
    },
    {
      "name": "Messaging",
      "item": [
        {
          "id": "b6b1756d-4cde-4bad-a436-7be445a3d82d",
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
              "id": "605b836b-73b0-4276-803f-c585a48fd68b"
            }
          ]
        },
        {
          "id": "cb58502c-0562-4a5e-a309-75541572a644",
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
              "id": "0b76ba0e-c941-4407-bb5d-38c99e8b0287"
            }
          ]
        }
      ]
    },
    {
      "name": "Smsmessaging",
      "item": [
        {
          "id": "80935f3e-9319-4f54-9adc-85166aae2c85",
          "name": "3smsmessaginginboundregistrationsregistrationidmessages",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.att.com",
              "path": [
                "3/smsmessaging/inbound/registrations/:registrationId/messages"
              ],
              "variable": [
                {
                  "id": "registrationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/3/smsmessaging/inbound/registrations/{registrationId}/messages"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d5bacb7-987d-4e8f-95bc-0b22e97c6089"
            }
          ]
        },
        {
          "id": "03dadf80-4f22-4790-8da4-2f0287313260",
          "name": "3smsmessagingoutboundrequestssenderaddressrequestiddeliveryinfos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.att.com",
              "path": [
                "3/smsmessaging/outbound/requests/:senderAddress/:requestId/deliveryInfos"
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
            "description": "/3/smsmessaging/outbound/requests/{senderAddress}/{requestId}/deliveryInfos"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef9cf271-b1f3-470d-b246-b4d3628b7cfe"
            }
          ]
        }
      ]
    }
  ]
}