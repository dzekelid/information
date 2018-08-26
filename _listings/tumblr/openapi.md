---
swagger: "2.0"
x-collection-name: Tumblr
x-complete: 1
info:
  title: Tumblr
  description: ntshare-photos-mobile-apps-and-social-network-using-tumblrs-apis-n----
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
---