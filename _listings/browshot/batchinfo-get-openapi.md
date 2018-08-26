---
swagger: "2.0"
x-collection-name: Browshot
x-complete: 0
info:
  title: Browshot Get the batch status
  description: Get the status of a batch requested through the API or through the
    dashboard.
  termsOfService: https://browshot.com/terms
  contact:
    name: API Support
    url: https://browshot.com/contact
    email: support@browshot.com
  version: 1.17.0
host: api.browshot.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/info:
    get:
      summary: Get information about your account
      description: Get information about your account.
      operationId: GetAccountInfo
      x-api-path-slug: accountinfo-get
      parameters:
      - in: query
        name: details
        description: level of information returned
      responses:
        200:
          description: OK
      tags:
      - Account
      - Info
  /batch/info:
    get:
      summary: Get the batch status
      description: Get the status of a batch requested through the API or through
        the dashboard.
      operationId: GetBatchInfo
      x-api-path-slug: batchinfo-get
      parameters:
      - in: query
        name: id
        description: batch ID
      responses:
        200:
          description: OK
      tags:
      - Batch
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