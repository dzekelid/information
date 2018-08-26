---
swagger: "2.0"
x-collection-name: AXA Assistance
x-complete: 0
info:
  title: AXA Assistance Gets the information linked to the policy holder of the home
    appliance damage declaration
  description: Gets the information linked to the policy holder of the home appliance
    damage declaration
  version: 1.0.0
host: sandbox.api.axa-assistance.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /information/version:
    get:
      summary: Provide basic details about the current deployed version of the information
        API
      description: Provide basic details about the current deployed version of the
        information API
      operationId: getInformationVersion
      x-api-path-slug: informationversion-get
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Provide
      - basic
      - detailAssistance
      - about
      - the
      - current
      - deployed
      - version
      - of
      - the
      - information
      - API
  /network/vexp/roadside_providers/{provider_id}:
    get:
      summary: Gets information of roadside provider.
      description: Gets information of roadside provider.
      operationId: getNetworkVexpRoadside_providersProvider_id
      x-api-path-slug: networkvexproadside-providersprovider-id-get
      parameters:
      - in: path
        name: provider_id
        description: Provider unique id
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - information
      - of
      - roadside
      - provider.
  /assistance/v1/home/glaziery_damage/declarations/{declaration_id}/policy_holders:
    get:
      summary: Gets the information linked to the policy holder of the glaziery damage
        declaration
      description: Gets the information linked to the policy holder of the glaziery
        damage declaration
      operationId: getAssistanceV1HomeGlaziery_damageDeclarationsDeclaration_idPolicy_holders
      x-api-path-slug: assistancev1homeglaziery-damagedeclarationsdeclaration-idpolicy-holders-get
      parameters:
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - the
      - information
      - linked
      - to
      - the
      - policy
      - holder
      - of
      - the
      - glaziery
      - damage
      - Declarations
  /assistance/v1/home/home_appliance_damage/declarations/{declaration_id}/policy_holders:
    get:
      summary: Gets the information linked to the policy holder of the home appliance
        damage declaration
      description: Gets the information linked to the policy holder of the home appliance
        damage declaration
      operationId: getAssistanceV1HomeHome_appliance_damageDeclarationsDeclaration_idPolicy_holders
      x-api-path-slug: assistancev1homehome-appliance-damagedeclarationsdeclaration-idpolicy-holders-get
      parameters:
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - the
      - information
      - linked
      - to
      - the
      - policy
      - holder
      - of
      - the
      - home
      - appliance
      - damage
      - Declarations
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