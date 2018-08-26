---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral Get Meeting Service Info
  description: "Returns information on dial-in numbers for meetings, support and international
    dial-in numbers URIs and meeting account information.\nApp Permission\nMeetings\nUser
    Permission\nMeetings\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n
    \  Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to call this
    API endpoint, application needs to have [Meetings] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [Meetings] permission for
    requested resource."
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/{apiVersion}:
    get:
      summary: Get Version Info
      description: |-
        Returns current API version info by apiVersion.
        Usage Plan Group
        NoThrottling
      operationId: getApiVersion
      x-api-path-slug: restapiapiversion-get
      parameters:
      - in: path
        name: apiVersion
        description: API version to be requested, for example v1
      responses:
        200:
          description: OK
      tags:
      - Version
      - Info
  /restapi/v1.0/glip/companies/{companyId}:
    get:
      summary: Get Company Info
      description: |-
        Returns a company by ID.
        App Permission
        Glip
        User Permission
        Glip
        Usage Plan Group
        Light
      operationId: loadGlipCompany
      x-api-path-slug: restapiv1-0glipcompaniescompanyid-get
      parameters:
      - in: path
        name: companyId
        description: Internal identifier of an RC account/Glip company, or tilde (~)
          to indicate a company the current user belongs to
      responses:
        200:
          description: OK
      tags:
      - Company
      - Info
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/meeting/{meetingId}:
    get:
      summary: Get Meeting Info [Beta]
      description: "Returns a particular meetings details by ID.\nApp Permission\nMeetings\nUser
        Permission\nMeetings\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP
        Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for
        parameter [meetingId] is not found"
      operationId: loadMeeting
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: meetingId
        description: Internal identifier of a RingCentral meeting
      responses:
        200:
          description: OK
      tags:
      - Meeting
      - Info
      - '[Beta]'
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/meeting/service-info:
    get:
      summary: Get Meeting Service Info
      description: "Returns information on dial-in numbers for meetings, support and
        international dial-in numbers URIs and meeting account information.\nApp Permission\nMeetings\nUser
        Permission\nMeetings\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP
        Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to
        call this API endpoint, application needs to have [Meetings] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [Meetings] permission
        for requested resource."
      operationId: loadMeetingServiceInfo
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmeetingserviceinfo-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - Meeting
      - Service
      - Info
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