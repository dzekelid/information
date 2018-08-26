---
swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 1
info:
  title: Broadleaf Commerce API
  description: the-default-broadleaf-commerce-apis
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /info:
    get:
      summary: Get Info
      description: Get info.
      operationId: getInfo
      x-api-path-slug: info-get
      responses:
        200:
          description: OK
      tags:
      - Info
  /info.json:
    get:
      summary: Get Info
      description: Get info.
      operationId: getInfo.json
      x-api-path-slug: info-json-get
      responses:
        200:
          description: OK
      tags:
      - Info
---