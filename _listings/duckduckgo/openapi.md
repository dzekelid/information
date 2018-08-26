---
swagger: "2.0"
x-collection-name: DuckDuckGo
x-complete: 1
info:
  title: No Title
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:
    get:
      summary: Search
      description: Our Zero-click Info API gives you free access to much of our topic
        summaries, categories, disambiguation, !bang redirects, definitions and more.
      operationId: zero-click-info
      x-api-path-slug: get
      parameters:
      - in: query
        name: callback
        description: Function to callback (for a JSONP formatted response)
      - in: query
        name: format
      - in: query
        name: no_html
        description: 1 to remove HTML from text, e
      - in: query
        name: no_redirect
        description: 1 to skip HTTP redirects (for !bang commands - see http://duckduckgo
      - in: query
        name: q
        description: Search terms
      - in: query
        name: skip_disambig
        description: 1 to skip disambiguation (D) Type
      responses:
        200:
          description: OK
      tags:
      - Search
---