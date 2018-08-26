---
swagger: "2.0"
x-collection-name: Actility
x-complete: 0
info:
  title: ThingPark DX Admin API Token Info Retrieval
  description: Retrieves information about a valid token.
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /admin/v140/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /oauth/tokeninfo:
    get:
      summary: Token Info Retrieval
      description: Retrieves information about a valid token.
      operationId: retrieves-information-about-a-valid-token
      x-api-path-slug: oauthtokeninfo-get
      parameters:
      - in: query
        name: access_token
        description: Value of the token for which info is requested
      responses:
        200:
          description: OK
      tags:
      - Token
      - Info
      - Retrieval
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