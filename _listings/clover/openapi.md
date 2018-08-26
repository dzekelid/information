---
swagger: "2.0"
x-collection-name: Clover
x-complete: 1
info:
  title: ""
  version: 1.0.0
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/apps/{aId}/merchants/{mId}/billing_info:
    get:
      summary: Get merchant's billing information for an app
      description: Gives detailed information about the status of the merchant's billing
        for the app including current subscription tier and trial status. Requires
        an OAuth generated token.
      operationId: GetMerchantBillingInfo
      x-api-path-slug: v3appsaidmerchantsmidbilling-info-get
      parameters:
      - in: path
        name: aId
        description: App Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        2:
          description: Successful response
        200:
          description: OK
      tags:
      - Apps
      - Merchants
      - Billing
      - Info
---