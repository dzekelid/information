{
  "info": {
    "name": "Plentymarkets Delete shipping information",
    "_postman_id": "2cfc42f2-d289-48d7-a277-bd55d80bef6c",
    "description": "Deletes the shipping information. The ID of the order must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Legal",
      "item": [
        {
          "id": "31503f38-8854-433b-9adc-625d4496e8c5",
          "name": "getRestLegalinformationPlentyLangType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/legalinformation/:plentyId/:lang/:type"
              ],
              "variable": [
                {
                  "id": "lang",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "plentyId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "type",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets legal information of an online store. The plenty ID of the store , the language and the type of legal information must be specified. The language must be specified as ISO 639-1 code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "caae7b8b-40ea-4ef8-a16c-74492e3f84f9"
            }
          ]
        }
      ]
    },
    {
      "name": "Coupon",
      "item": [
        {
          "id": "2b400d64-9ffe-4edd-a9bb-d35771b55b66",
          "name": "getRestOrdersCouponsCampaignsCodesCode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/coupons/campaigns/codes/:code"
              ],
              "query": [
                {
                  "key": "with",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets coupon code information. The code must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7fa0e363-35ca-492f-b6c3-488761112d62"
            }
          ]
        }
      ]
    },
    {
      "name": "Shipping",
      "item": [
        {
          "id": "7e99cd9a-f2ac-4e98-97e1-4106b32a6f20",
          "name": "postRestOrdersShippingShippingInformation",
          "request": {
            "url": "http://example.com/rest/orders/shipping/shipping_information",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Create shipping information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "709b3649-8f54-40b4-aba5-77d840ac53dc"
            }
          ]
        },
        {
          "id": "77d7c5df-550a-4db2-ab40-e343ac96a231",
          "name": "deleteRestOrdersOrderShippingShippingInformation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/:orderId/shipping/shipping_information"
              ],
              "variable": [
                {
                  "id": "orderId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the shipping information. The ID of the order must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ec364d7-d203-4147-a4bd-346def2cd001"
            }
          ]
        }
      ]
    }
  ]
}