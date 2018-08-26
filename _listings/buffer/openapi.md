---
swagger: "2.0"
x-collection-name: Buffer
x-complete: 1
info:
  title: Bufferapp
  description: social-media-management-for-marketers-and-agencies
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
---