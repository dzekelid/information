---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/ApplicationInfo:
    get:
      summary: Get API Application Information
      description: Get api application information.
      operationId: ApiApplicationInfoGet
      x-api-path-slug: apiapplicationinfo-get
      responses:
        200:
          description: OK
      tags:
      - Application
      - Information
  /api/ExchangeInfo:
    get:
      summary: Get API Exchangeinfo
      description: Get api exchangeinfo.
      operationId: ApiExchangeInfoGet
      x-api-path-slug: apiexchangeinfo-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: exchangeId
      responses:
        200:
          description: OK
      tags:
      - Exchangeinfo
  /api/MyLykkeInfo:
    get:
      summary: Get API Mylykkeinfo
      description: Get api mylykkeinfo.
      operationId: ApiMyLykkeInfoGet
      x-api-path-slug: apimylykkeinfo-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Mylykkeinfo
  /api/TransferInfo:
    get:
      summary: Get API Transferinfo
      description: Get api transferinfo.
      operationId: ApiTransferInfoGet
      x-api-path-slug: apitransferinfo-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: transferId
      responses:
        200:
          description: OK
      tags:
      - Transferinfo
---