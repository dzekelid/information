---
swagger: "2.0"
x-collection-name: Infermedica
x-complete: 1
info:
  title: Infermedica
  description: empower-your-healthcare-services-with-intelligent-diagnostic-insights-of-infermedica-api-
  version: v2
host: api.infermedica.com
basePath: /v1
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
      description: Returns information about data used by diagnostic engine.
      operationId: getInfo
      x-api-path-slug: info-get
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Info
---