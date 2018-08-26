---
swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 0
info:
  title: AWS Storage Gateway Service API Describe Gateway Information
  version: 1.0.0
  description: |-
    Returns metadata about a gateway such as its name, network interfaces, configured
             time zone, and the state (whether the gateway is running or not).
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeGatewayInformation:
    get:
      summary: Describe Gateway Information
      description: |-
        Returns metadata about a gateway such as its name, network interfaces, configured
                 time zone, and the state (whether the gateway is running or not).
      operationId: describeGatewayInformation
      x-api-path-slug: actiondescribegatewayinformation-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateway
  /?Action=UpdateGatewayInformation:
    get:
      summary: Update Gateway Information
      description: Updates a gateway's metadata, which includes the gateway's name
        and time zone.
      operationId: updateGatewayInformation
      x-api-path-slug: actionupdategatewayinformation-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: GatewayName
        description: The name you configured for your gateway
        type: string
      - in: query
        name: GatewayTimezone
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateway
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