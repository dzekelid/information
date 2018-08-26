---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Get API Application Information
  version: 1.0.0
  description: Get api application information.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/ApplicationInfo:
    get:
      summary: Get API Application Information
      description: Get api application information.
      operationId: ApiApplicationInfoGet
      x-api-path-slug: apiapplicationinfo-get
      responses:
        200:
          description: OK
      tags:
      - Application
      - Information
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