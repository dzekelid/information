{
  "info": {
    "name": "Plentymarkets Update additional data of the shipping information",
    "_postman_id": "c968d023-b0dc-48fb-95ff-87702eb6daee",
    "description": "Updates additional data of the shipping information. The ID of the order must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Legal",
      "item": [
        {
          "id": "690d6445-903e-4ddd-afa9-765762a62265",
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
              "id": "f8271dfc-c07c-416c-b42f-7f51703edd08"
            }
          ]
        }
      ]
    },
    {
      "name": "Coupon",
      "item": [
        {
          "id": "3572c730-6388-433c-88f4-04857f86481a",
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
              "id": "41398cb7-6416-4651-9f1d-8467852e77a5"
            }
          ]
        }
      ]
    },
    {
      "name": "Shipping",
      "item": [
        {
          "id": "66282cfa-c5f9-4582-9ade-640153a9bda3",
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
              "id": "b53755f9-6c30-4478-925c-1052e3863877"
            }
          ]
        },
        {
          "id": "89b97b4c-398b-49d6-9223-4614a57f7ba4",
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
              "id": "673868d3-1bcf-4654-a010-0a0570270415"
            }
          ]
        },
        {
          "id": "98768d16-b0c4-4708-81a2-ab2825275974",
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
              "id": "1c8f140a-808c-44b7-b08c-fc89746d3c91"
            }
          ]
        }
      ]
    },
    {
      "name": "Additional",
      "item": [
        {
          "id": "82eef265-3b8c-43a4-8c76-b900b2b9a5aa",
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
              "id": "45fe2b59-851d-498e-902e-02b33f50e43b"
            }
          ]
        }
      ]
    }
  ]
}