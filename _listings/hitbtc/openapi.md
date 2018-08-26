---
swagger: "2.0"
x-collection-name: HitBTC
x-complete: 1
info:
  title: HitBTC API
  description: create-api-keys-in-your-profile-httpshitbtc-comsettingsapikeys-and-use-public-api-key-as-username-and-secret-as-password-to-authorize-
  version: 1.0.0
basePath: /api/2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /public/symbol/{symbol}:
    get:
      summary: Get Symbol Info
      description: Get symbol info.
      operationId: getPublicSymbolSymbol
      x-api-path-slug: publicsymbolsymbol-get
      parameters:
      - in: path
        name: symbol
      responses:
        200:
          description: OK
      tags:
      - Symbol
      - Info
  /public/currency/{currency}:
    get:
      summary: Get Currency Info
      description: Get currency info.
      operationId: getPublicCurrencyCurrency
      x-api-path-slug: publiccurrencycurrency-get
      parameters:
      - in: path
        name: currency
      responses:
        200:
          description: OK
      tags:
      - Currency
      - Info
---