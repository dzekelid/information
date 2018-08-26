---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 0
info:
  title: Stack Exchange Get Information
  description: "Returns a collection of statistics about the site.\n \nData to facilitate
    per-site customization, discover related sites, and aggregate statistics is all
    returned by this method.\n \nThis data is cached very aggressively, by design.
    Query sparingly, ideally no more than once an hour.\n \nThis method returns an
    info object."
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /info:
    get:
      summary: Get Information
      description: "Returns a collection of statistics about the site.\n \nData to
        facilitate per-site customization, discover related sites, and aggregate statistics
        is all returned by this method.\n \nThis data is cached very aggressively,
        by design. Query sparingly, ideally no more than once an hour.\n \nThis method
        returns an info object."
      operationId: returns-a-collection-of-statistics-about-the-site-data-to-facilitate-persite-customization-discover-
      x-api-path-slug: info-get
      parameters:
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
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