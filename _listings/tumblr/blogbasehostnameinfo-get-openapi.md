---
swagger: "2.0"
x-collection-name: Tumblr
x-complete: 0
info:
  title: Tumblr Get Blog Base Hostname Info
  description: This method returns general information about the blog, such as the
    title, number of posts, and other high-level data.
  version: 1.0.0
host: api.tumblr.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /blog/{base-hostname}/info:
    get:
      summary: Get Blog Base Hostname Info
      description: This method returns general information about the blog, such as
        the title, number of posts, and other high-level data.
      operationId: blog.base_hostname.info.get
      x-api-path-slug: blogbasehostnameinfo-get
      parameters:
      - in: path
        name: base-hostname
        description: The unique hostname of the blog
      responses:
        200:
          description: OK
      tags:
      - Blog
      - Base
      - Hostname
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