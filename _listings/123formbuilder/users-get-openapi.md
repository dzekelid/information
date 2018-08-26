---
swagger: "2.0"
x-collection-name: 123FormBuilder
x-complete: 0
info:
  title: 123FormBuilder Get info about master user and subusers
  version: 1.0.0
  description: Get info about master user and subusers
host: api.123contactform.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users:
    get:
      summary: Get info about master user and subusers
      description: Get info about master user and subusers
      operationId: get-info-about-master-user-and-subusers
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: JWT
        description: JWT authentication token
      - in: query
        name: page
        description: Page number
      - in: query
        name: per_page
        description: The number of groups to get per page in a request
      responses:
        200:
          description: OK
      tags:
      - Info
      - About
      - Master
      - User
      - Subusers
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