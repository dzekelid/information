---
swagger: "2.0"
x-collection-name: Quovo
x-complete: 1
info:
  title: Quovo API v3
  description: todo-add-description
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{account_id}/extras:
    get:
      summary: Fetch an Account's Extras Information
      description: Retrieves an Account's Extras Information.
      operationId: AccountsExtrasByAccountIdGet
      x-api-path-slug: accountsaccount-idextras-get
      parameters:
      - in: path
        name: account_id
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - Accounts
      - Extras
      - Information
  /me:
    get:
      summary: Get info about your API user
      description: Fetch information about your Quovo API user.
      operationId: MeGet
      x-api-path-slug: me-get
      responses:
        200:
          description: OK
      tags:
      - Info
      - About
      - Your
      - User
---