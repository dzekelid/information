---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get server info
  description: Returns general information about the current Jira server.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/serverInfo:
    get:
      summary: Get server info
      description: Returns general information about the current Jira server.
      operationId: com.atlassian.jira.rest.v2.ServerInfoResource.getServerInfo_get
      x-api-path-slug: api2serverinfo-get
      responses:
        200:
          description: OK
      tags:
      - Server
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