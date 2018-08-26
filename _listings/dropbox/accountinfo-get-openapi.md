---
swagger: "2.0"
x-collection-name: Dropbox
x-complete: 0
info:
  title: Dropbox Core Retrieves information about the user's account.
  description: Retrieves information about the user's account.
  termsOfService: https://www.dropbox.com/developers/reference/tos
  contact:
    name: Dropbox
    url: https://www.dropbox.com/developers
  version: 1.0.0
host: api.dropbox.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/info:
    get:
      summary: Retrieves information about the user's account.
      description: Retrieves information about the user's account.
      operationId: retrieves-information-about-the-users-account
      x-api-path-slug: accountinfo-get
      parameters:
      - in: query
        name: locale
        description: Use to specify language settings for user error messages and
          other language specific text
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Documents
      - Account
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