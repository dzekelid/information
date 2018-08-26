---
swagger: "2.0"
x-collection-name: ATTOM
x-complete: 0
info:
  title: Attom Data Solutions API Returns detailed property information and most recent
    transaction and taxes.
  description: Get a detailed property information and most recent transaction and
    taxes for a specific address.
  version: 1.0.0
host: search.onboard-apis.com
basePath: /communityapi/v2.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /property/basicprofile:
    get:
      summary: Returns basic property information and most recent transaction and
        taxes.
      description: Get basic property information and most recent transaction and
        taxes for a specific attom id.
      operationId: propertyBasicProfile
      x-api-path-slug: propertybasicprofile-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: attomid
        description: attom id
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Basic
      - Property
      - Information
      - Most
      - Recent
      - Transaction
      - Taxes
  /property/expandedprofile:
    get:
      summary: Returns detailed property information and most recent transaction and
        taxes.
      description: Get a detailed property information and most recent transaction
        and taxes for a specific address.
      operationId: propertyExpandedProfile
      x-api-path-slug: propertyexpandedprofile-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: Application Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Detailed
      - Property
      - Information
      - Most
      - Recent
      - Transaction
      - Taxes
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