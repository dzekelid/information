---
swagger: "2.0"
x-collection-name: Mynewsdesk
x-complete: 1
info:
  title: My News Desk Pressroom List
  description: mynewsdesk-webservice-for-newsroom-is-a-way-for-you-as-a-registered-customer-to-fetch-information-from-your-newsroom-at-mynewsdesk-to-any-system--you-can-get-all-your-information-as-xml-and-create-email-subscriptions-to-your-material-
  termsOfService: http://www.mynewsdesk.com/about/terms-and-conditions?locale=en
  version: v1
host: www.mynewsdesk.com
basePath: /services/pressroom/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  pressroom_info/:
    get:
      summary: Pressroom Info
      description: Pressroom Info
      operationId: getPressroomInfo
      x-api-path-slug: pressroom-info-get
      parameters:
      - in: query
        name: pressroom
        description: Set the pressroom to search in
      - in: path
        name: unique key
        description: The MyNewsDesk API Key
      responses:
        200:
          description: OK
      tags:
      - News
      - Pressroom
      - Info
---