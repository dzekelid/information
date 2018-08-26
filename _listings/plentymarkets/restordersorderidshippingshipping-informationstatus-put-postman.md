{
  "info": {
    "name": "Plentymarkets Update the shipping status of the shipping information",
    "_postman_id": "f9e47eb9-006b-4d98-a3a4-ff5bdb42c70b",
    "description": "Updates the shipping status of the shipping information. The ID of the order must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Legal",
      "item": [
        {
          "id": "173ae6b3-3117-4659-a373-6cfd23a96a9b",
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
              "id": "aaf33632-a7b4-4b9f-8529-a20b3342438d"
            }
          ]
        }
      ]
    },
    {
      "name": "Coupon",
      "item": [
        {
          "id": "3f799109-c202-4492-a0ab-ba05d3c3d0cf",
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
              "id": "a10ed868-df70-447e-a7bd-7fbfd52c0431"
            }
          ]
        }
      ]
    },
    {
      "name": "Shipping",
      "item": [
        {
          "id": "8ddf705d-229a-4fc6-96e7-a9f7a4a64479",
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
              "id": "9aaa4342-2fff-4cda-8f53-7879e2c3b340"
            }
          ]
        },
        {
          "id": "fe698b44-f341-45e0-866c-52601ce2ce01",
          "name": "getRestOrdersOrderShippingShippingInformation",
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
            "description": "Gets the shipping information. The ID of the order must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8013ab1-3d8a-4e5a-8687-568e766c8cee"
            }
          ]
        },
        {
          "id": "f2ae4cc2-c370-4235-9403-f034a116086a",
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
              "id": "b7822c98-7238-4847-8b14-bba9e2ca1611"
            }
          ]
        },
        {
          "id": "4babb89c-fbda-4f62-a7a2-68143595b6a2",
          "name": "putRestOrdersOrderShippingShippingInformationStatus",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/:orderId/shipping/shipping_information/status"
              ],
              "variable": [
                {
                  "id": "orderId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
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
            "description": "Updates the shipping status of the shipping information. The ID of the order must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11a94e84-9d3e-4336-a6ec-49aeb52a92d3"
            }
          ]
        }
      ]
    },
    {
      "name": "Additional",
      "item": [
        {
          "id": "f0219bc8-aad7-4f29-a716-6bf8d2f85445",
          "name": "putRestOrdersOrderShippingShippingInformationAdditionalData",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/:orderId/shipping/shipping_information/additional_data"
              ],
              "variable": [
                {
                  "id": "orderId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
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
            "description": "Updates additional data of the shipping information. The ID of the order must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15d88012-3285-4151-b665-bc399dc4fa3d"
            }
          ]
        }
      ]
    }
  ]
}