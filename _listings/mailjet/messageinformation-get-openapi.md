---
swagger: "2.0"
x-collection-name: Mailjet
x-complete: 0
info:
  title: Mailjet Messages API Message Information
  description: Lists the information about a message.
  version: v3
host: api.mailjet.com
basePath: v3/REST/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  messageinformation/:
    get:
      summary: Message Information
      description: Lists the information about a message.
      operationId: getMessageinformation
      x-api-path-slug: messageinformation-get
      parameters:
      - in: query
        name: CampaignID
        description: Unique numerical ID for this object
      - in: query
        name: CampaignStatus
        description: Only retrieve campaigns with status equal to specified value
      - in: query
        name: ContactsList
        description: Only retrieve campaigns sent to specified Contacts list
      - in: query
        name: CustomCampaign
        description: Only retrieve campaigns with given Custom Value
      - in: query
        name: From
        description: Only retrieve campaigns with given From header
      - in: query
        name: FromDomain
        description: Only retrieve campaigns with given domain in From header
      - in: query
        name: FromID
        description: Only retrieve campaigns with this sender ID
      - in: query
        name: FromTS
        description: Only retrieve campaigns with SendStartAt after this timestamp
      - in: query
        name: FromType
        description: Only retrieve campaigns with FromType equal to specified value
      - in: query
        name: IsDeleted
        description: Only retrieve campaigns where isDeleted matches the specified
          value
      - in: query
        name: IsNewsletterTool
        description: Only retrieve campaigns which were started by the newsletter
          tool
      - in: query
        name: IsStarred
        description: Only retrieve campaigns which were marked as starred
      - in: query
        name: MessageStatus
        description: Only retrieve messages with status equal to specified value
      - in: query
        name: Period
        description: Set FromTS and ToTS timestamps to beginning of indicated period
          and current timestamp, respectively
      - in: query
        name: ToTS
        description: Only retrieve campaigns with SendStartAt timestamp less than
          the specified value
      responses:
        200:
          description: OK
      tags:
      - Message
      - Information
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