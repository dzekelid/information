---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Confluence Cloud API Get system info
  description: "Returns the system information for the Confluence Cloud tenant. This\ninformation
    is used by Atlassian.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to access the Confluence site ('Can use' global permission)."
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
  /settings/systemInfo:
    get:
      summary: Get system info
      description: "Returns the system information for the Confluence Cloud tenant.
        This\ninformation is used by Atlassian.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to access the Confluence site ('Can use' global permission)."
      operationId: com.atlassian.confluence.plugins.restapi.resources.SystemInfoResource.getSystemInfo_get
      x-api-path-slug: settingssysteminfo-get
      responses:
        200:
          description: OK
      tags:
      - System
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