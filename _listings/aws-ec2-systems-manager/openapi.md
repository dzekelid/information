---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 1
info:
  title: AWS EC2 Systems Manager API
  version: 1.0.0
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
---