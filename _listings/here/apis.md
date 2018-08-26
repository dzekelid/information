---
name: HERE
x-slug: here
description: HERE Technologies enables people, enterprises and cities around the world
  to harness the power of location and create innovative solutions that make our lives
  safer and more efficient. We transform information from devices, vehicles, infrastructure
  and...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
x-kinRank: "7"
x-alexaRank: "3011"
tags: Information
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/information/master/_listings/here/apis.md
specificationVersion: "0.14"
apis:
- name: Geocoder API - Geocode using partial address information
  x-api-slug: geocode-json-get
  description: "*Request the latitude, longitude and details of an address based on
    partial address information*\n\nThis example shows a structured (qualified) geocoding
    request using the `geocode` endpoint. In this structured request the data is provided
    in `country`, `city`, `street` and `housenumber` parameters in the request URL.
    Note that the street name misses the directional (\"W\") and also the street type.
    The omitted directional makes the query ambiguous and the response contains therefore
    two results: One address on West Randolph St and one on East Randolph St.\n  \n\n\n\n*
    **housenumber**  `text`\n \\- The house number or house name\n\n* **street**  `text`\n
    \\- The street name can include suite, apt and floor information.\n\n* **city**
    \ `text`\n \\- City name\n\n* **country**  `text`\n \\- Specify the country or
    list of countries using the country code (3 bytes, ISO 3166-1-alpha-3) or the
    country name\n\n* **gen**  `number`\n \\- Enables/disables backward incompatible
    behavior in the API\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded
    string used for the authentication of the client application.    You must include
    an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64
    URL-safe encoded string used for the authentication of the client application.
    \   You must include an `app_code` with every request."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://geocoder.cit.api.here.com//6.2
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/information/master/_listings/here/geocode-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/information/master/_listings/here/geocode-json-get-openapi.md
- name: Map Tile API - Copyright Information
  x-api-slug: copyrightnewest-get
  description: "*Request map tile copyright information*\n\nTo make a request for
    copyright information, use the `copyright` parameter in the path of the request
    URL.\n  \n  Note that the client-side process formatting the JSON response may
    take some time in older browsers.\n\n\n\n* **app_id**  `text`\n \\- A 20 byte
    Base64 URL-safe encoded string used for the authentication of the client application.
    \   You must include an `app_id` with every request.\n\n* **app_code**  `text`\n
    \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the
    client application.    You must include an `app_code` with every request."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://1.aerial.maps.cit.api.here.com//maptile/2.1/maptile/newest
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/information/master/_listings/here/copyrightnewest-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/information/master/_listings/here/copyrightnewest-get-openapi.md
- name: Map Tile API - Map Tile Type Information
  x-api-slug: info-get
  description: |-
    *Request information about the types of map tiles available on a server*

    To make a request for metadata information, use the `info` parameter in the path of the request URL.



    * **output**  `enum`
     \- Indicates whether to return the information in XML format, JSON format or as an XML schema (XSD) of the API metadata

     Valid values are : `json`, `xml`, `xsd`

    * **app_id**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

    * **app_code**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://1.aerial.maps.cit.api.here.com//maptile/2.1/maptile/newest
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/information/master/_listings/here/info-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/information/master/_listings/here/info-get-openapi.md
- name: Routing API - Link Information using linkId
  x-api-slug: getlinkinfo-json-get
  description: "*Request detailed information about a path segment in the routing
    network given a linkid*\n\nLink information can be retrieved using the `getlinkinfo`
    endpoint, by specifying one or more comma separated linkIds using the `linkids`
    parameter. The `linkids` have been generated from a previous request. Note that
    positive direction '+' in link Ids has to be URL encoded.\n  \n  \n\n\n\n* **linkids**
    \ `text`\n \\- Link identifiers for which the detailed information is being requested.\n\n*
    **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the
    authentication of the client application.    You must include an `app_id` with
    every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded
    string used for the authentication of the client application.    You must include
    an `app_code` with every request."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://route.cit.api.here.com//routing/7.2
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/information/master/_listings/here/getlinkinfo-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/information/master/_listings/here/getlinkinfo-json-get-openapi.md
- name: Routing API - Previously calculated route information
  x-api-slug: getroute-json-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://route.cit.api.here.com//routing/7.2
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/information/master/_listings/here/getroute-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/information/master/_listings/here/getroute-json-get-openapi.md
x-common:
- type: x-blog-rss
  url: https://developer.here.com/blog/feed
- type: x-github
  url: https://github.com/heremaps
- type: x-postman-collection
  url: https://github.com/heremaps/postman-collections
- type: x-api-gallery
  url: http://healthcare.gov.api.gallery.streamdata.io
- type: x-api-stack
  url: http://here.stack.network
- type: x-blog
  url: https://developer.here.com/blog
- type: x-crunchbase
  url: https://crunchbase.com/organization/here-inc
- type: x-developer
  url: https://developer.here.com
- type: x-email
  url: dirk.popp@here.com
- type: x-email
  url: sebastian.kurme@here.com
- type: x-email
  url: jordan.stark@here.com
- type: x-email
  url: amy.stupavsky@here.com
- type: x-email
  url: minna.laub@here.com
- type: x-email
  url: stefanie.sirc@here.com
- type: x-email
  url: rachel.kuta@here.com
- type: x-email
  url: laurel.davis-lyons@here.com
- type: x-email
  url: linda.bradley@here.com
- type: x-email
  url: press@here.com
- type: x-twitter
  url: https://twitter.com/here
- type: x-website
  url: https://here.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---