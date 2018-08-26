---
swagger: "2.0"
x-collection-name: ATTOM
x-complete: 0
info:
  title: Attom Data Solutions API Returns home sale information for properties within
    a geography.
  description: Get a list of home sale snapshots within a Onboard GeoID that sold
    within a date range and specified sale amount.
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
  /area/full:
    get:
      summary: Returns community information.
      description: This search returns community information for a specific geography.
      operationId: getCommunityAPIAreaFull
      x-api-path-slug: areafull-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: ApiKey
        description: Application Key
      - in: query
        name: AreaId
        description: This is the Area ID to search
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Community
      - Information
  /sale/detail:
    get:
      summary: Returns sale information for a property.
      description: Get sales information for a specific address.
      operationId: getSaleDetailPostal
      x-api-path-slug: saledetail-get
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
      - Sale
      - Informationa
      - Property
  /sale/snapshot:
    get:
      summary: Returns home sale information for properties within a geography.
      description: Get a list of home sale snapshots within a Onboard GeoID that sold
        within a date range and specified sale amount.
      operationId: getHomeSaleSnapshotsGeoId
      x-api-path-slug: salesnapshot-get
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
      - in: query
        name: endsalesearchdate
        description: The standardized date for search purposes
      - in: query
        name: geoid
        description: A list of geographies that this property belongs to
      - in: query
        name: maxsaleamt
        description: The recorded amount of the sale transaction
      - in: query
        name: minsaleamt
        description: The recorded amount of the sale transaction
      - in: query
        name: propertytype
        description: A specific property classification such as Detached Single Family
      - in: query
        name: radius
      - in: query
        name: startsalesearchdate
        description: The standardized date for search purposes
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Home
      - Sale
      - Informationproperties
      - Within
      - Geography
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