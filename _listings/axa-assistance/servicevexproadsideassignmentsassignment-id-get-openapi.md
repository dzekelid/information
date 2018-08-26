---
swagger: "2.0"
x-collection-name: AXA Assistance
x-complete: 0
info:
  title: AXA Assistance Gets assignment information.
  description: Gets assignment information.
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
  /assistance/v1/home/locksmithing_damage/declarations/{declaration_id}/policy_holders:
    get:
      summary: Gets the information linked to the policy holder of the locksmithing
        damage declaration
      description: Gets the information linked to the policy holder of the locksmithing
        damage declaration
      operationId: getAssistanceV1HomeLocksmithing_damageDeclarationsDeclaration_idPolicy_holders
      x-api-path-slug: assistancev1homelocksmithing-damagedeclarationsdeclaration-idpolicy-holders-get
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
      - locksmithing
      - damage
      - Declarations
  /assistance/v1/home/water_damage/declarations/{declaration_id}/policy_holders:
    get:
      summary: Gets the information related to each the policy holder of the water
        damage declaration
      description: Gets the information related to each the policy holder of the water
        damage declaration
      operationId: getAssistanceV1HomeWater_damageDeclarationsDeclaration_idPolicy_holders
      x-api-path-slug: assistancev1homewater-damagedeclarationsdeclaration-idpolicy-holders-get
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
      - related
      - to
      - each
      - the
      - policy
      - holder
      - of
      - the
      - water
      - damage
      - Declarations
  /assistance/v1/home/electric_damage/declarations/{declaration_id}/contacts:
    post:
      summary: Adds contact information of the electric damage declaration
      description: Adds contact information of the electric damage declaration
      operationId: postAssistanceV1HomeElectric_damageDeclarationsDeclaration_idContacts
      x-api-path-slug: assistancev1homeelectric-damagedeclarationsdeclaration-idcontacts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - contact
      - information
      - of
      - the
      - electric
      - damage
      - Declarations
  /assistance/v1/home/gas_damage/declarations/{declaration_id}/contacts:
    post:
      summary: Adds contact information of the gas damage declaration
      description: Adds contact information of the gas damage declaration
      operationId: postAssistanceV1HomeGas_damageDeclarationsDeclaration_idContacts
      x-api-path-slug: assistancev1homegas-damagedeclarationsdeclaration-idcontacts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - contact
      - information
      - of
      - the
      - gaAssistance
      - damage
      - Declarations
  /assistance/v1/home/glaziery_damage/declarations/{declaration_id}/contacts:
    post:
      summary: Adds contact information of the glaziery damage declaration
      description: Adds contact information of the glaziery damage declaration
      operationId: postAssistanceV1HomeGlaziery_damageDeclarationsDeclaration_idContacts
      x-api-path-slug: assistancev1homeglaziery-damagedeclarationsdeclaration-idcontacts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - contact
      - information
      - of
      - the
      - glaziery
      - damage
      - Declarations
  /assistance/v1/home/home_appliance_damage/declarations/{declaration_id}/contacts:
    post:
      summary: Adds contact information of the home appliance damage declaration
      description: Adds contact information of the home appliance damage declaration
      operationId: postAssistanceV1HomeHome_appliance_damageDeclarationsDeclaration_idContacts
      x-api-path-slug: assistancev1homehome-appliance-damagedeclarationsdeclaration-idcontacts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - contact
      - information
      - of
      - the
      - home
      - appliance
      - damage
      - Declarations
  /assistance/v1/home/locksmithing_damage/declarations/{declaration_id}/contacts:
    post:
      summary: Adds contact information of the locksmithing damage declaration
      description: Adds contact information of the locksmithing damage declaration
      operationId: postAssistanceV1HomeLocksmithing_damageDeclarationsDeclaration_idContacts
      x-api-path-slug: assistancev1homelocksmithing-damagedeclarationsdeclaration-idcontacts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - contact
      - information
      - of
      - the
      - locksmithing
      - damage
      - Declarations
  /assistance/v1/home/water_damage/declarations/{declaration_id}/contacts:
    post:
      summary: Adds contact information of the water damage declaration
      description: Adds contact information of the water damage declaration
      operationId: postAssistanceV1HomeWater_damageDeclarationsDeclaration_idContacts
      x-api-path-slug: assistancev1homewater-damagedeclarationsdeclaration-idcontacts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - contact
      - information
      - of
      - the
      - water
      - damage
      - Declarations
  /assistance/v1/home/electric_damage/declarations/{declaration_id}:
    patch:
      summary: Updates information related to the electric damage declaration
      description: Updates information related to the electric damage declaration
      operationId: patchAssistanceV1HomeElectric_damageDeclarationsDeclaration_id
      x-api-path-slug: assistancev1homeelectric-damagedeclarationsdeclaration-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - information
      - related
      - to
      - the
      - electric
      - damage
      - Declarations
  /assistance/v1/home/gas_damage/declarations/{declaration_id}:
    patch:
      summary: Updates information related to the gas damage declaration
      description: Updates information related to the gas damage declaration
      operationId: patchAssistanceV1HomeGas_damageDeclarationsDeclaration_id
      x-api-path-slug: assistancev1homegas-damagedeclarationsdeclaration-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - information
      - related
      - to
      - the
      - gaAssistance
      - damage
      - Declarations
  /assistance/v1/home/glaziery_damage/declarations/{declaration_id}:
    patch:
      summary: Updates information related to the glaziery damage declaration
      description: Updates information related to the glaziery damage declaration
      operationId: patchAssistanceV1HomeGlaziery_damageDeclarationsDeclaration_id
      x-api-path-slug: assistancev1homeglaziery-damagedeclarationsdeclaration-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - information
      - related
      - to
      - the
      - glaziery
      - damage
      - Declarations
  /assistance/v1/home/home_appliance_damage/declarations/{declaration_id}:
    patch:
      summary: Updates information related to the home appliance damage declaration
      description: Updates information related to the home appliance damage declaration
      operationId: patchAssistanceV1HomeHome_appliance_damageDeclarationsDeclaration_id
      x-api-path-slug: assistancev1homehome-appliance-damagedeclarationsdeclaration-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - information
      - related
      - to
      - the
      - home
      - appliance
      - damage
      - Declarations
  /assistance/v1/home/locksmithing_damage/declarations/{declaration_id}:
    patch:
      summary: Updates information related to the locksmithing damage declaration
      description: Updates information related to the locksmithing damage declaration
      operationId: patchAssistanceV1HomeLocksmithing_damageDeclarationsDeclaration_id
      x-api-path-slug: assistancev1homelocksmithing-damagedeclarationsdeclaration-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - information
      - related
      - to
      - the
      - locksmithing
      - damage
      - Declarations
  /assistance/v1/home/water_damage/declarations/{declaration_id}:
    patch:
      summary: Updates information related to the water damage declaration
      description: Updates information related to the water damage declaration
      operationId: patchAssistanceV1HomeWater_damageDeclarationsDeclaration_id
      x-api-path-slug: assistancev1homewater-damagedeclarationsdeclaration-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - information
      - related
      - to
      - the
      - water
      - damage
      - Declarations
  /assistance/v1/home/electric_damage/declarations/{declaration_id}/policy_holders/{policy_holder_id}:
    patch:
      summary: Updates the policy holder information of the electric damage declaration
      description: Updates the policy holder information of the electric damage declaration
      operationId: patchAssistanceV1HomeElectric_damageDeclarationsDeclaration_idPolicy_holdersPolicy_holder_id
      x-api-path-slug: assistancev1homeelectric-damagedeclarationsdeclaration-idpolicy-holderspolicy-holder-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      - in: path
        name: policy_holder_id
        description: ID of the policy holder
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - the
      - policy
      - holder
      - information
      - of
      - the
      - electric
      - damage
      - Declarations
  /assistance/v1/home/gas_damage/declarations/{declaration_id}/policy_holders/{policy_holder_id}:
    patch:
      summary: Updates the policy holder information of the gas damage declaration
      description: Updates the policy holder information of the gas damage declaration
      operationId: patchAssistanceV1HomeGas_damageDeclarationsDeclaration_idPolicy_holdersPolicy_holder_id
      x-api-path-slug: assistancev1homegas-damagedeclarationsdeclaration-idpolicy-holderspolicy-holder-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      - in: path
        name: policy_holder_id
        description: ID of the policy holder
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - the
      - policy
      - holder
      - information
      - of
      - the
      - gaAssistance
      - damage
      - Declarations
  /assistance/v1/home/glaziery_damage/declarations/{declaration_id}/policy_holders/{policy_holder_id}:
    patch:
      summary: Updates the policy holder information of the glaziery damage declaration
      description: Updates the policy holder information of the glaziery damage declaration
      operationId: patchAssistanceV1HomeGlaziery_damageDeclarationsDeclaration_idPolicy_holdersPolicy_holder_id
      x-api-path-slug: assistancev1homeglaziery-damagedeclarationsdeclaration-idpolicy-holderspolicy-holder-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      - in: path
        name: policy_holder_id
        description: ID of the policy holder
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - the
      - policy
      - holder
      - information
      - of
      - the
      - glaziery
      - damage
      - Declarations
  /assistance/v1/home/home_appliance_damage/declarations/{declaration_id}/policy_holders/{policy_holder_id}:
    patch:
      summary: Update the policy holder information of the home appliance damage declaration
      description: Update the policy holder information of the home appliance damage
        declaration
      operationId: patchAssistanceV1HomeHome_appliance_damageDeclarationsDeclaration_idPolicy_holdersPolicy_holder_id
      x-api-path-slug: assistancev1homehome-appliance-damagedeclarationsdeclaration-idpolicy-holderspolicy-holder-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      - in: path
        name: policy_holder_id
        description: ID of the policy holder
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - the
      - policy
      - holder
      - information
      - of
      - the
      - home
      - appliance
      - damage
      - Declarations
  /assistance/v1/home/locksmithing_damage/declarations/{declaration_id}/policy_holders/{policy_holder_id}:
    patch:
      summary: Updates the policy holder information of the locksmithing damage declaration
      description: Updates the policy holder information of the locksmithing damage
        declaration
      operationId: patchAssistanceV1HomeLocksmithing_damageDeclarationsDeclaration_idPolicy_holdersPolicy_holder_id
      x-api-path-slug: assistancev1homelocksmithing-damagedeclarationsdeclaration-idpolicy-holderspolicy-holder-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      - in: path
        name: policy_holder_id
        description: ID of the policy holder
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - the
      - policy
      - holder
      - information
      - of
      - the
      - locksmithing
      - damage
      - Declarations
  /assistance/v1/home/water_damage/declarations/{declaration_id}/policy_holders/{policy_holder_id}:
    patch:
      summary: Updates the policy holder information of the water damage declaration
      description: Updates the policy holder information of the water damage declaration
      operationId: patchAssistanceV1HomeWater_damageDeclarationsDeclaration_idPolicy_holdersPolicy_holder_id
      x-api-path-slug: assistancev1homewater-damagedeclarationsdeclaration-idpolicy-holderspolicy-holder-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: declaration_id
        description: ID of the declaration
      - in: path
        name: policy_holder_id
        description: ID of the policy holder
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - the
      - policy
      - holder
      - information
      - of
      - the
      - water
      - damage
      - Declarations
  /sales/v1/individual/car_rental/certificates:
    post:
      summary: Requests the activation of a car rental certificate linked to a product.
        At least one product_criteria has to be specified to identify the product
        to which to subscribe. If the user already holds a certificate, this api will
        update its personal infor
      description: Requests the activation of a car rental certificate linked to a
        product. At least one product_criteria has to be specified to identify the
        product to which to subscribe. If the user already holds a certificate, this
        api will update its personal infor
      operationId: postSalesV1IndividualCar_rentalCertificates
      x-api-path-slug: salesv1individualcar-rentalcertificates-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - the
      - activation
      - ofcar
      - rental
      - certificate
      - linked
      - toproduct.
      - At
      - leastproduct_criteria
      - haAssistance
      - to
      - be
      - specified
      - to
      - identify
      - the
      - product
      - to
      - which
      - to
      - subscribe.
      - If
      - the
      - user
      - already
      - holdscertificate
      - ""
      - thiAssistance
      - api
      - will
      - update
      - itAssistance
      - personal
      - infor
  /sales/v1/individual/travel/certificates:
    post:
      summary: Requests the activation of a travel certificate linked to a product.
        At least one product_criteria has to be specified to identify the product
        to which to subscribe. If the user already holds a certificate, this api will
        update its personal informati
      description: Requests the activation of a travel certificate linked to a product.
        At least one product_criteria has to be specified to identify the product
        to which to subscribe. If the user already holds a certificate, this api will
        update its personal informati
      operationId: postSalesV1IndividualTravelCertificates
      x-api-path-slug: salesv1individualtravelcertificates-post
      parameters:
      - in: header
        name: accept-language
        description: Accepted language, IANA language codification
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - RequestAssistance
      - the
      - activation
      - oftravel
      - certificate
      - linked
      - toproduct.
      - At
      - leastproduct_criteria
      - haAssistance
      - to
      - be
      - specified
      - to
      - identify
      - the
      - product
      - to
      - which
      - to
      - subscribe.
      - If
      - the
      - user
      - already
      - holdscertificate
      - ""
      - thiAssistance
      - api
      - will
      - update
      - itAssistance
      - personal
      - informati
  /service/vexp/roadside/assignments/{assignment_id}:
    get:
      summary: Gets assignment information.
      description: Gets assignment information.
      operationId: getServiceVexpRoadsideAssignmentsAssignment_id
      x-api-path-slug: servicevexproadsideassignmentsassignment-id-get
      parameters:
      - in: path
        name: assignment_id
        description: Assignment unique identifier
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Assistance
      - assignment
      - information.
  /information/v1/countries/{country_id}/security_cards:
    get:
      summary: Retrieve security information for a country
      description: Retrieve security information for a country
      operationId: getInformationV1CountriesCountry_idSecurity_cards
      x-api-path-slug: informationv1countriescountry-idsecurity-cards-get
      parameters:
      - in: header
        name: accept-language
        description: Language/Country
      - in: path
        name: country_id
        description: country id
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Retrieve
      - security
      - informationa
      - country
  /information/v1/countries/{country_id}/health_cards:
    get:
      summary: Retrieve health information for a country
      description: Retrieve health information for a country
      operationId: getInformationV1CountriesCountry_idHealth_cards
      x-api-path-slug: informationv1countriescountry-idhealth-cards-get
      parameters:
      - in: header
        name: accept-language
        description: Language/Country
      - in: path
        name: country_id
        description: country id
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Retrieve
      - health
      - informationa
      - country
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