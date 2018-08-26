---
swagger: "2.0"
x-collection-name: Cloud Elements
x-complete: 0
info:
  title: Cloud Elements - Dropbox For Business API Get Member Info
  description: Get member info.
  version: "1"
host: api.dropbox.com
basePath: /1/team
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /get_info:
    post:
      summary: Get Info
      description: Get info.
      operationId: postGetInfo
      x-api-path-slug: get-info-post
      responses:
        200:
          description: OK
      tags:
      - Info
  /members/get_info:
    post:
      summary: Get Member Info
      description: Get member info.
      operationId: postMembersGetInfo
      x-api-path-slug: membersget-info-post
      parameters:
      - in: query
        name: email
        description: optional email of member
      - in: query
        name: external_id
        description: optional external ID of member
      - in: query
        name: member_id
        description: optional ID of member
      responses:
        200:
          description: OK
      tags:
      - Member
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