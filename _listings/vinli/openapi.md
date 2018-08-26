---
swagger: "2.0"
x-collection-name: Vinli
x-complete: 1
info:
  title: Vinli
  description: todo-add-description
  version: 1.0.0
host: events.vin.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /codes:
    get:
      summary: Get Info about a DTC
      description: Get info about a dtc.
      operationId: CodesGet
      x-api-path-slug: codes-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: number
      responses:
        200:
          description: OK
      tags:
      - Info
      - About
      - DTC
---