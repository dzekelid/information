---
swagger: "2.0"
x-collection-name: BMC Software
x-complete: 1
info:
  title: BMC Software Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account:
    get:
      summary: Account Resource
      description: Information about the authorized account.
      operationId: information-about-the-authorized-account
      x-api-path-slug: account-get
      responses:
        200:
          description: OK
      tags:
      - Account
---