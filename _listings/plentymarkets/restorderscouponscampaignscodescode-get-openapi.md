---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Get coupon code information
  description: Gets coupon code information. The code must be specified.
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