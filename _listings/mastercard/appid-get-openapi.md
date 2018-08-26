---
swagger: "2.0"
x-collection-name: MasterCard
x-complete: 0
info:
  title: Mastercard Get App
  description: |-
    Information about an application referenced by the `id` parameter. If
    you are permissioned to that application, this will also return the
    message definitions you will need to comply with to issue valid transaction
    entries for that application.
  version: 1.0.0
host: eas5stl0.mastercard.int:13046
basePath: /z0/core/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /address/{address}:
    get:
      summary: Get Address Address
      description: |-
        Information about a particular address on the network. Note that this
        call may return information about a blockchain node or a signing entity.
        Also, the level of detail returned will vary depending on your permissions
        for the query target.
      operationId: getAddressAddress
      x-api-path-slug: addressaddress-get
      parameters:
      - in: path
        name: address
      - in: header
        name: MCWSSAML
        description: SAML Authorization
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Address
      - Address
  /app/{id}:
    get:
      summary: Get App
      description: |-
        Information about an application referenced by the `id` parameter. If
        you are permissioned to that application, this will also return the
        message definitions you will need to comply with to issue valid transaction
        entries for that application.
      operationId: getApp
      x-api-path-slug: appid-get
      parameters:
      - in: path
        name: id
      - in: header
        name: MCWSSAML
        description: SAML Authorization
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - App
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