---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/appointment/freebusy:
    post:
      summary: Returns Free/Busy information regarding multiple people.
      description: Returns free/busy information regarding multiple people..
      operationId: Appointment_GetFreeBusyByquery
      x-api-path-slug: apiappointmentfreebusy-post
      parameters:
      - in: body
        name: query
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Free
      - Busy
      - Information
      - Regarding
      - Multiple
      - People
  /api/documentgeneration/custompack:
    post:
      summary: Generates any correspondence and can allow you to overpost information
        to the correspondence
      description: Generates any correspondence and can allow you to overpost information
        to the correspondence.
      operationId: DocumentGeneration_GeneratePackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcustompack-post
      parameters:
      - in: body
        name: generatePackDetails
        description: broad contract that allows for overposting and underposting,
          however you must specify a correspondence Id            you must then follow
          the validation rules for the for that individual correspondence type, each
          route to the controller is named in the same way            as the enumerated
          correspondence type system name, and the mappings for the specific class
          to the GeneratePackJobDataContract are detailed in             the each
          individual simplified contract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Any
      - Correspondence
      - Can
      - Ow
      - You
      - To
      - Overpost
      - Information
      - To
      - Correspondence
  /api/role/lettings/{id}/setlettinginfo:
    post:
      summary: Sets the core information on a letting role
      description: Sets the core information on a letting role.
      operationId: LettingRole_SetInfoByidBydatacontract
      x-api-path-slug: apirolelettingsidsetlettinginfo-post
      parameters:
      - in: body
        name: datacontract
        description: The letting information of the role
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The role id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Core
      - Information
      - "On"
      - Letting
      - Role
  /api/documentgeneration/headertemplates:
    get:
      summary: Returns a list of header templates associated to this agency with their
        associated brand info
      description: Returns a list of header templates associated to this agency with
        their associated brand info.
      operationId: DocumentGeneration_GetPrintableHeaderTemplates
      x-api-path-slug: apidocumentgenerationheadertemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Header
      - Templates
      - Associated
      - To
      - This
      - Agency
      - Their
      - Associated
      - Brand
      - Info
  /api/group/{id}/saveadditionalinfo:
    put:
      summary: To save or edit the Group additional info i.e. the Origin and Grade.
      description: To save or edit the group additional info i.e. the origin and grade..
      operationId: Group_SaveAdditionalInfoByidBysaveAdditionalInfoDataContract
      x-api-path-slug: apigroupidsaveadditionalinfo-put
      parameters:
      - in: path
        name: id
        description: The group id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: saveAdditionalInfoDataContract
        description: The additional info to set on the group i
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - To
      - Save
      - Edit
      - Group
      - Additional
      - Info
      - I
      - E
      - ""
      - Origin
      - Grade
  /api/progression/lettings/{tenantInfoId}/detachrighttorentdocument/{documentId}:
    put:
      summary: Detach
      description: Detach.
      operationId: LettingsProgression_DetachRightToRentDocumentBytenantInfoIdBydocumentId
      x-api-path-slug: apiprogressionlettingstenantinfoiddetachrighttorentdocumentdocumentid-put
      parameters:
      - in: path
        name: documentId
        description: The document Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: tenantInfoId
        description: The tenant info Id
      responses:
        200:
          description: OK
      tags:
      - Detach
---