---
swagger: "2.0"
x-collection-name: Etsy
x-complete: 1
info:
  title: Etsy
  description: bring-etsys-handmade-marketplace-and-community-into-your-apps-
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /listings/{listing_id}/shipping/info:
    get:
      summary: Get Listings Listing Shipping Info
      description: Retrieves a set of ShippingInfo objects associated to a Listing.
      operationId: getListingsListingShippingInfo
      x-api-path-slug: listingslisting-idshippinginfo-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: listing_id
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Shipping
      - Info
    post:
      summary: Post Listings Listing Shipping Info
      description: Creates a new ShippingInfo.
      operationId: postListingsListingShippingInfo
      x-api-path-slug: listingslisting-idshippinginfo-post
      parameters:
      - in: query
        name: destination_country_id
      - in: path
        name: listing_id
      - in: query
        name: origin_country_id
      - in: query
        name: primary_cost
      - in: query
        name: region_id
      - in: query
        name: secondary_cost
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Shipping
      - Info
  /shipping/info/{shipping_info_id}:
    get:
      summary: Get Shipping Info Shipping Info
      description: Retrieves a ShippingInfo by id.
      operationId: getShippingInfoShippingInfo
      x-api-path-slug: shippinginfoshipping-info-id-get
      parameters:
      - in: path
        name: shipping_info_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Info
      - Shipping
      - Info
    put:
      summary: Put Shipping Info Shipping Info
      description: Updates a ShippingInfo with the given id.
      operationId: putShippingInfoShippingInfo
      x-api-path-slug: shippinginfoshipping-info-id-put
      parameters:
      - in: query
        name: destination_country_id
      - in: query
        name: listing_id
      - in: query
        name: origin_country_id
      - in: query
        name: primary_cost
      - in: query
        name: region_id
      - in: query
        name: secondary_cost
      - in: path
        name: shipping_info_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Info
      - Shipping
      - Info
    delete:
      summary: Delete Shipping Info Shipping Info
      description: Deletes the ShippingInfo with the given id.
      operationId: deleteShippingInfoShippingInfo
      x-api-path-slug: shippinginfoshipping-info-id-delete
      parameters:
      - in: path
        name: shipping_info_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Info
      - Shipping
      - Info
---