---
swagger: "2.0"
x-collection-name: AWS EC2 Container Registry Service
x-complete: 1
info:
  title: AWS EC2 Container Registry API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CompleteLayerUpload:
    get:
      summary: Complete Layer Upload
      description: Inform Amazon ECR that the image layer upload for a specified registry,
        repository name, and upload ID, has completed.
      operationId: completeLayerUpload
      x-api-path-slug: actioncompletelayerupload-get
      responses:
        200:
          description: OK
      tags:
      - Layer Upload
---