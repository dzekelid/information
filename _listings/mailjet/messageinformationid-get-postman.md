{
  "info": {
    "name": "Mailjet Messages API Message Information",
    "_postman_id": "d9cd9d8b-cf48-43c3-8288-4f52a24ea410",
    "description": "Lists a message informaiton.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Message",
      "item": [
        {
          "id": "9973efc9-e58b-4403-94d5-d40ae9f3cfda",
          "name": "getMessage",
          "request": {
            "url": "http://api.mailjet.com/v3/REST/message/?Campaign=%7B%7D&Contact=%7B%7D&MessageState=%7B%7D&PlanSubscription=%7B%7D&Sender=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows you to list messages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89de85f5-db7d-4313-ab6d-5961b0903a99"
            }
          ]
        },
        {
          "id": "e6e86ed5-4768-4fe3-bc6f-e723740f5d62",
          "name": "getMessagehistory",
          "request": {
            "url": "http://api.mailjet.com/v3/REST/messagehistory/?Message=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List message history resources"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "21fb8502-ee89-4057-90e5-c075bafc8817"
            }
          ]
        },
        {
          "id": "dd7a06de-7c17-4150-bb33-b62c4b4e0b7e",
          "name": "getMessagehistory",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailjet.com",
              "path": [
                "v3",
                "REST",
                "messagehistory/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the history of a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cfc33314-48c9-44a3-aa3f-381ef8d4dcf7"
            }
          ]
        },
        {
          "id": "af673d8c-8ee9-4d4c-bd9d-4527e825c22d",
          "name": "getMessageinformation",
          "request": {
            "url": "http://api.mailjet.com/v3/REST/messageinformation/?CampaignID=%7B%7D&CampaignStatus=%7B%7D&ContactsList=%7B%7D&CustomCampaign=%7B%7D&From=%7B%7D&FromDomain=%7B%7D&FromID=%7B%7D&FromTS=%7B%7D&FromType=%7B%7D&IsDeleted=%7B%7D&IsNewsletterTool=%7B%7D&IsStarred=%7B%7D&MessageStatus=%7B%7D&Period=%7B%7D&ToTS=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the information about a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1b542af-e272-4af7-b8b0-15c072125861"
            }
          ]
        },
        {
          "id": "644d45ea-5e54-48be-ba1e-590c689f45ac",
          "name": "getMessageinformation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailjet.com",
              "path": [
                "v3",
                "REST",
                "messageinformation/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists a message informaiton."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a1f77bb-02e4-4617-a33b-99e7d0c27c76"
            }
          ]
        }
      ]
    }
  ]
}