---
swagger: "2.0"
x-collection-name: CoinFabrik
x-complete: 1
info:
  title: Coinbase API
  description: the-coinbase-v2-api
  contact:
    name: CoinFabrik
    url: http://www.coinfabrik.com/
  version: 1.0.0
host: api.coinbase.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/auth:
    get:
      summary: Show authorization information
      description: "Get current user\u2019s authorization information including granted
        scopes and send limits when using OAuth2 authentication."
      operationId: get-current-users-authorization-information-including-granted-scopes-and-send-limits-when-using-oaut
      x-api-path-slug: userauth-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Show
      - Authorization
      - Information
---