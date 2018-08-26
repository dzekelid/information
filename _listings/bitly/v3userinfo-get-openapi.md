---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 0
info:
  title: Bitly User API User Info
  description: Return or update information about a user.
  termsOfService: http://dev.bitly.com/best_practices.html
  version: v3
host: api-ssl.bitly.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/user/info:
    get:
      summary: User Info
      description: Return or update information about a user.
      operationId: userInfo
      x-api-path-slug: v3userinfo-get
      parameters:
      - in: query
        name: full_name
        description: set the users full name value
      - in: query
        name: login
        description: the bitly login of the user whose info to look up
      responses:
        200:
          description: OK
      tags:
      - User
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