---
swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 1
info:
  title: HPE OneSphere API
  description: hpe-onesphere-hybrid-cloud-management-rest-api-for-calls-requiring-authentication-use-restsession-to-get-a-token-
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /onboarding/azure/provider-info:
    get:
      summary: Get Onboarding Azure Prover Info
      description: Returns the provider information required to add an Azure provider
      operationId: getAzureProviderInfo
      x-api-path-slug: onboardingazureproviderinfo-get
      parameters:
      - in: query
        name: directoryUri
        description: The Azure Directory URI associated with the SubscriptionFor Example:myActiveDirectory
      - in: query
        name: location
        description: The full response Azure sends to the redirectURI including valid
          Azure authentication codeFor Example:https://customername
      responses:
        200:
          description: OK
      tags:
      - Onboarding
      - Azure
      - Prover
      - Info
---