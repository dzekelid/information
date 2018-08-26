---
swagger: "2.0"
x-collection-name: AWS Elastic Beanstalk
x-complete: 1
info:
  title: AWS Elastic Beanstalk API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RequestEnvironmentInfo:
    get:
      summary: Request Environment Info
      description: |-
        Initiates a request to compile the specified type of information of the deployed
              environment.
      operationId: requestEnvironmentInfo
      x-api-path-slug: actionrequestenvironmentinfo-get
      parameters:
      - in: query
        name: EnvironmentId
        description: The ID of the environment of the requested data
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment of the requested data
        type: string
      - in: query
        name: InfoType
        description: The type of information to request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=RetrieveEnvironmentInfo:
    get:
      summary: Retrieve Environment Info
      description: Retrieves the compiled information from a.
      operationId: retrieveEnvironmentInfo
      x-api-path-slug: actionretrieveenvironmentinfo-get
      parameters:
      - in: query
        name: EnvironmentId
        description: The ID of the datas environment
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the datas environment
        type: string
      - in: query
        name: InfoType
        description: The type of information to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
---