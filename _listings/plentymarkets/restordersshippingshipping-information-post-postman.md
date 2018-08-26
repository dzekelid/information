{
  "info": {
    "name": "Plentymarkets Create shipping information",
    "_postman_id": "cfec94db-9142-4b7f-9b51-0794f783f8c0",
    "description": "Create shipping information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Legal",
      "item": [
        {
          "id": "d6463500-55cc-4c05-882f-2bea8357fd47",
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
              "id": "8d101d72-083b-4d2e-9db6-c4edf26fcb81"
            }
          ]
        }
      ]
    },
    {
      "name": "Coupon",
      "item": [
        {
          "id": "ac33fecb-9f38-411f-a4a5-3ec1eab7d60d",
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
              "id": "ae35fc00-dc02-41e3-902c-8c4e89f039ab"
            }
          ]
        }
      ]
    },
    {
      "name": "Shipping",
      "item": [
        {
          "id": "924e8603-d1b9-4ecc-93c8-ba19574a8949",
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
              "id": "a81baaf4-b26c-4f40-bd2d-80acc35c3990"
            }
          ]
        }
      ]
    }
  ]
}