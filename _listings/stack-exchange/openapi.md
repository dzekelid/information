---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 1
info:
  title: Stack Exchange
  description: stack-exchange-is-a-network-of-130-qa-communities-including-stack-overflow-
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
  /tags/{tags}/info:
    get:
      summary: Get Tags Info
      description: "Returns tag objects representing the tags in {tags} found on the
        site.\n \nThis method diverges from the standard naming patterns to avoid
        to conflicting with existing methods, due to the free form nature of tag names.\n
        \nThis method returns a list of tags.\n \nThe sorts accepted by this method
        operate on the follow fields of the tag object:\n - popular - count\n - activity
        - the creation_date of the last question asked with the tag\n - name - name\n
        \ popular is the default sort.\n \n It is possible to create moderately complex
        queries using sort, min, max, fromdate, and todate."
      operationId: returns-tag-objects-representing-the-tags-in-tags-found-on-the-site-this-method-diverges-from-the-st
      x-api-path-slug: tagstagsinfo-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: min
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: path
        name: tags
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Information
---