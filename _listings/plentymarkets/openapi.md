---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
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
    put:
      summary: Save legal information for an online store
      description: |-
        Saves a legal information for an online store. The plenty ID of the online store, the language of the legal information and the type of the legal information must be specified. The language must be specified as ISO 639-1 code.
        Existing legal information will be overwritten.
      operationId: putRestLegalinformationPlentyLangType
      x-api-path-slug: restlegalinformationplentyidlangtype-put
      parameters:
      - in: body
        name: /rest/legalinformation/{plentyId}/{lang}/{type}
        schema:
          $ref: '#/definitions/holder'
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
      - Save
      - Legal
      - Informationan
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
  /rest/storage/frontend/file:
    get:
      summary: Get file information for a single object in frontend storage. Append
        public cloudfront url to retrieved object.
      description: Get file information for a single object in frontend storage. append
        public cloudfront url to retrieved object..
      operationId: getRestStorageFrontendFile
      x-api-path-slug: reststoragefrontendfile-get
      parameters:
      - in: query
        name: key
        description: The key of the object to get information about
      responses:
        200:
          description: OK
      tags:
      - File
      - Informationa
      - Single
      - Object
      - In
      - Frontend
      - Storage
      - ""
      - Append
      - Public
      - Cloudfront
      - Url
      - To
      - Retrieved
      - Object
  /rest/listings/markets/infos:
    get:
      summary: Search listing market info
      description: Search listing market info by filter options.
      operationId: getRestListingsMarketsInfos
      x-api-path-slug: restlistingsmarketsinfos-get
      parameters:
      - in: query
        name: code
        description: Filter that restricts the search result to listing market info
          with given codes
      - in: query
        name: createdAtFrom
        description: Filter that restricts the search result to listing markets that
          were last updated on the specified date
      - in: query
        name: createdAtTo
        description: Filter that restricts the search result to listing markets that
          were last updated within a specified period of time
      - in: query
        name: id
        description: Filter that restricts the search result to listing market info
          that match the given ID(s)
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: listingMarketId
        description: Filter that restricts the search result to listing market info
          that match the given listing market ID(s)
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: type
        description: Filter that restricts the search result to listing market info
          with a custom type
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Search
      - Listing
      - Market
      - Info
---