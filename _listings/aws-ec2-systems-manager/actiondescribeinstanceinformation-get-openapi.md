---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API Describe Instance Information
  version: 1.0.0
  description: Describes one or more of your instances.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeInstanceInformation:
    get:
      summary: Describe Instance Information
      description: Describes one or more of your instances.
      operationId: describeInstanceInformation
      x-api-path-slug: actiondescribeinstanceinformation-get
      parameters:
      - in: query
        name: Filters
        description: One or more filters
        type: string
      - in: query
        name: InstanceInformationFilterList
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
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