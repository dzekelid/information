---
swagger: "2.0"
x-collection-name: Dropbox
x-complete: 0
info:
  title: Cloud Elements - Dropbox For Business API Get Info Batch
  description: Get info batch.
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
  /members/get_info_batch:
    post:
      summary: Get Info Batch
      description: Get info batch.
      operationId: postMembersGetInfoBatch
      x-api-path-slug: membersget-info-batch-post
      parameters:
      - in: query
        name: emails
        description: optional list of member emails
      - in: query
        name: external_ids
        description: optional list of external member IDs
      - in: query
        name: member_ids
        description: optional list of member IDs
      responses:
        200:
          description: OK
      tags:
      - Info
      - Batch
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