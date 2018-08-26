---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Update the shipping status of the shipping information
  description: Updates the shipping status of the shipping information. The ID of
    the order must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/legalinformation/{plentyId}/{lang}/{type}:
    get:
      summary: Get legal information of an online store
      description: Gets legal information of an online store. The plenty ID of the
        store , the language and the type of legal information must be specified.
        The language must be specified as ISO 639-1 code.
      operationId: getRestLegalinformationPlentyLangType
      x-api-path-slug: restlegalinformationplentyidlangtype-get
      parameters:
      - in: path
        name: lang
      - in: path
        name: plentyId
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - Legal
      - Information
      - Of
      - Online
      - Store
  /rest/orders/coupons/campaigns/codes/{code}:
    get:
      summary: Get coupon code information
      description: Gets coupon code information. The code must be specified.
      operationId: getRestOrdersCouponsCampaignsCodesCode
      x-api-path-slug: restorderscouponscampaignscodescode-get
      parameters:
      - in: path
        name: code
      - in: query
        name: with
        description: Load additional relations for a coupon code
      responses:
        200:
          description: OK
      tags:
      - Coupon
      - Code
      - Information
  /rest/orders/shipping/shipping_information:
    post:
      summary: Create shipping information
      description: Create shipping information.
      operationId: postRestOrdersShippingShippingInformation
      x-api-path-slug: restordersshippingshipping-information-post
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Information
  /rest/orders/{orderId}/shipping/shipping_information:
    delete:
      summary: Delete shipping information
      description: Deletes the shipping information. The ID of the order must be specified.
      operationId: deleteRestOrdersOrderShippingShippingInformation
      x-api-path-slug: restordersorderidshippingshipping-information-delete
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Information
    get:
      summary: Get shipping information
      description: Gets the shipping information. The ID of the order must be specified.
      operationId: getRestOrdersOrderShippingShippingInformation
      x-api-path-slug: restordersorderidshippingshipping-information-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Information
  /rest/orders/{orderId}/shipping/shipping_information/additional_data:
    put:
      summary: Update additional data of the shipping information
      description: Updates additional data of the shipping information. The ID of
        the order must be specified.
      operationId: putRestOrdersOrderShippingShippingInformationAdditionalData
      x-api-path-slug: restordersorderidshippingshipping-informationadditional-data-put
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Additional
      - Data
      - Of
      - Shipping
      - Information
  /rest/orders/{orderId}/shipping/shipping_information/status:
    put:
      summary: Update the shipping status of the shipping information
      description: Updates the shipping status of the shipping information. The ID
        of the order must be specified.
      operationId: putRestOrdersOrderShippingShippingInformationStatus
      x-api-path-slug: restordersorderidshippingshipping-informationstatus-put
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Status
      - Of
      - Shipping
      - Information
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---