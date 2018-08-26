---
swagger: "2.0"
x-collection-name: Buffer
x-complete: 0
info:
  title: Buffer Get Info Configuration Mediatypeextension
  description: Returns an object with the current configuration that Buffer is using,
    including supported services, their icons and the varying limits of character
    and schedules.
  version: "1"
host: api.bufferapp.com
basePath: /1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /info/configuration{mediaTypeExtension}:
    get:
      summary: Get Info Configuration Mediatypeextension
      description: Returns an object with the current configuration that Buffer is
        using, including supported services, their icons and the varying limits of
        character and schedules.
      operationId: returns-an-object-with-the-current-configuration-that-buffer-is-using-including-supported-services-t
      x-api-path-slug: infoconfigurationmediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
      responses:
        200:
          description: OK
      tags:
      - Info
      - ConfigurationmediaTypeExtension
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