---
swagger: "2.0"
x-collection-name: HERE
x-complete: 0
info:
  title: HERE Routing API Previously calculated route information
  description: "*Request information about a previously calculated route*\n\nPrevious
    routes can be retrieved using the `getroute` endpoint and appending a `routeid`
    to the request. The `routeid` in question has been generated from a previous request.
    Note that server map updates usually invalidates `routeid` value computed on previous
    map versions. If it is the case, the `routeid` computation should be requested
    again on the map in current  use.\n  \n\n\n\n* **mode**  `text`\n \\- Routing
    mode determines how the route is calculated.    e.g. `fastest;car;traffic:disabled.`
    \ \n\n* **routeid**  `text`\n \\- Route identifier for which the detailed route
    information is being requested.  \n\n* **app_id**  `text`\n \\- A 20 byte Base64
    URL-safe encoded string used for the authentication of the client application.
    \   You must include an `app_id` with every request.  \n\n* **app_code**  `text`\n
    \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the
    client application.    You must include an `app_code` with every request."
  version: 1.0.0
host: route.cit.api.here.com
basePath: /routing/7.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /getlinkinfo.json:
    get:
      summary: Link Information using linkId
      description: "*Request detailed information about a path segment in the routing
        network given a linkid*\n\nLink information can be retrieved using the `getlinkinfo`
        endpoint, by specifying one or more comma separated linkIds using the `linkids`
        parameter. The `linkids` have been generated from a previous request. Note
        that positive direction '+' in link Ids has to be URL encoded.\n  \n  \n\n\n\n*
        **linkids**  `text`\n \\- Link identifiers for which the detailed information
        is being requested.\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe
        encoded string used for the authentication of the client application.    You
        must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\-
        A 20 byte Base64 URL-safe encoded string used for the authentication of the
        client application.    You must include an `app_code` with every request."
      operationId: GetlinkinfoJsonGet2
      x-api-path-slug: getlinkinfo-json-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: linkids
      responses:
        200:
          description: OK
      tags:
      - Link
      - Information
      - Using
      - LinkId
  /getroute.json:
    get:
      summary: Previously calculated route information
      description: "*Request information about a previously calculated route*\n\nPrevious
        routes can be retrieved using the `getroute` endpoint and appending a `routeid`
        to the request. The `routeid` in question has been generated from a previous
        request. Note that server map updates usually invalidates `routeid` value
        computed on previous map versions. If it is the case, the `routeid` computation
        should be requested again on the map in current  use.\n  \n\n\n\n* **mode**
        \ `text`\n \\- Routing mode determines how the route is calculated.    e.g.
        `fastest;car;traffic:disabled.`  \n\n* **routeid**  `text`\n \\- Route identifier
        for which the detailed route information is being requested.  \n\n* **app_id**
        \ `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication
        of the client application.    You must include an `app_id` with every request.
        \ \n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string
        used for the authentication of the client application.    You must include
        an `app_code` with every request."
      operationId: GetrouteJsonGet
      x-api-path-slug: getroute-json-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: mode
      - in: query
        name: routeid
      responses:
        200:
          description: OK
      tags:
      - Previously
      - Calculated
      - Route
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