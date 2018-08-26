---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /about:
    get:
      summary: About
      description: Information about this API, such as Version code, etc
      operationId: about
      x-api-path-slug: about-get
      responses:
        200:
          description: OK
      tags:
      - About
---