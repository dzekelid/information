---
swagger: "2.0"
x-collection-name: AT&T Dev Program
x-complete: 0
info:
  title: AT&T API Get Devices Info
  description: /rest/2/Devices/Info
  version: "1"
host: api.att.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /myMessages/v2/messages/index/info:
    get:
      summary: Get My Messages Index Info
      description: /myMessages/v2/messages/index/info
      operationId: mymessagesv2messagesindexinfo
      x-api-path-slug: mymessagesv2messagesindexinfo-get
      responses:
        200:
          description: OK
      tags:
      - MyMessages
      - VMessages
      - Index
      - Info
  /rest/2/Devices/Info:
    get:
      summary: Get Devices Info
      description: /rest/2/Devices/Info
      operationId: rest2devicesinfo
      x-api-path-slug: rest2devicesinfo-get
      responses:
        200:
          description: OK
      tags:
      - Rest
      - Devices
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