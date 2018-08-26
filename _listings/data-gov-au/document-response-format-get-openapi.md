---
swagger: "2.0"
x-collection-name: Data.Gov.au
x-complete: 0
info:
  title: Regulations.gov Returns Document information
  description: Returns document information.
  version: "3.0"
host: api.data.gov
basePath: /regulations/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /docket.{response_format}:
    get:
      summary: Returns Docket information
      description: Returns docket information.
      operationId: getDocket.ResponseFormat
      x-api-path-slug: docket-response-format-get
      parameters:
      - in: query
        name: docketId
        description: Docket ID
      - in: path
        name: response_format
        description: Format
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Docket
      - Information
  /document.{response_format}:
    get:
      summary: Returns Document information
      description: Returns document information.
      operationId: getDocument.ResponseFormat
      x-api-path-slug: document-response-format-get
      parameters:
      - in: query
        name: documentId
        description: FDMS Document ID
      - in: query
        name: federalRegisterNumber
        description: Federal Register Document Number
      - in: path
        name: response_format
        description: Format
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Document
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