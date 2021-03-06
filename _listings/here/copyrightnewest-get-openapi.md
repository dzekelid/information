---
swagger: "2.0"
x-collection-name: HERE
x-complete: 0
info:
  title: HERE Map Tile API Copyright Information
  description: "*Request map tile copyright information*\n\nTo make a request for
    copyright information, use the `copyright` parameter in the path of the request
    URL.\n  \n  Note that the client-side process formatting the JSON response may
    take some time in older browsers.\n\n\n\n* **app_id**  `text`\n \\- A 20 byte
    Base64 URL-safe encoded string used for the authentication of the client application.
    \   You must include an `app_id` with every request.\n\n* **app_code**  `text`\n
    \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the
    client application.    You must include an `app_code` with every request."
  version: 1.0.0
host: 1.aerial.maps.cit.api.here.com
basePath: /maptile/2.1/maptile/newest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /copyright/newest:
    get:
      summary: Copyright Information
      description: "*Request map tile copyright information*\n\nTo make a request
        for copyright information, use the `copyright` parameter in the path of the
        request URL.\n  \n  Note that the client-side process formatting the JSON
        response may take some time in older browsers.\n\n\n\n* **app_id**  `text`\n
        \\- A 20 byte Base64 URL-safe encoded string used for the authentication of
        the client application.    You must include an `app_id` with every request.\n\n*
        **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for
        the authentication of the client application.    You must include an `app_code`
        with every request."
      operationId: CopyrightNewestGet
      x-api-path-slug: copyrightnewest-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      responses:
        200:
          description: OK
      tags:
      - Copyright
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