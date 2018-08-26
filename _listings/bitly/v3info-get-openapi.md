---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 0
info:
  title: Bitly Link API Get Info
  description: Get info.
  termsOfService: http://dev.bitly.com/best_practices.html
  version: "3.0"
host: api-ssl.bitly.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/info:
    get:
      summary: Get Info
      description: Get info.
      operationId: getV3Info
      x-api-path-slug: v3info-get
      parameters:
      - in: query
        name: expand_user
        description: optional true|false - include extra user info in response
      - in: query
        name: hash
        description: refers to one or more bitly hashes, (e
      - in: query
        name: shortUrl
        description: refers to one or more Bitlinks e
      responses:
        200:
          description: OK
      tags:
      - Info
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