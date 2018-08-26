---
swagger: "2.0"
x-collection-name: Mynewsdesk
x-complete: 0
info:
  title: My News Desk Pressroom List Pressroom Info
  description: Pressroom Info
  termsOfService: http://www.mynewsdesk.com/about/terms-and-conditions?locale=en
  version: v1
host: www.mynewsdesk.com
basePath: /services/pressroom/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  pressroom_info/:
    get:
      summary: Pressroom Info
      description: Pressroom Info
      operationId: getPressroomInfo
      x-api-path-slug: pressroom-info-get
      parameters:
      - in: query
        name: pressroom
        description: Set the pressroom to search in
      - in: path
        name: unique key
        description: The MyNewsDesk API Key
      responses:
        200:
          description: OK
      tags:
      - News
      - Pressroom
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