---
swagger: "2.0"
x-collection-name: PayRun
x-complete: 1
info:
  title: Pay Run.IO
  description: open-scableable-transparent-payroll-api-
  version: 17.18.6.206
host: api.test.payrun.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Jobs/Dps/{JobId}/Info:
    get:
      summary: Get the DPS job information
      description: Return the the DPS job information
      operationId: GetDpsJobInfo
      x-api-path-slug: jobsdpsjobidinfo-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - DPJob
      - Information
  /Jobs/PayRuns/{JobId}/Info:
    get:
      summary: Get the pay run job information
      description: Return the the payrun job information
      operationId: GetPayRunJobInfo
      x-api-path-slug: jobspayrunsjobidinfo-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Job
      - Information
  /Jobs/Rti/{JobId}/Info:
    get:
      summary: Get the RTI job information
      description: Return the the RTI job information
      operationId: GetRtiJobInfo
      x-api-path-slug: jobsrtijobidinfo-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - RTI
      - Job
      - Information
  /Templates/applicationinfo:
    get:
      summary: Gets the application info template
      description: Return the application info data object template
      operationId: GetApplicationInfoTemplate
      x-api-path-slug: templatesapplicationinfo-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Application
      - Info
      - Template
  /Templates/jobinfo:
    get:
      summary: Gets the job info template
      description: Return the job info data object template
      operationId: GetJobInfoTemplate
      x-api-path-slug: templatesjobinfo-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Job
      - Info
      - Template
---