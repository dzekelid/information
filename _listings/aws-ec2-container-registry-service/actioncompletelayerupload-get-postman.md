{
  "info": {
    "name": "AWS EC2 Container Registry API Complete Layer Upload",
    "_postman_id": "f9c4cf20-8bc3-49a9-9a28-8f9dbda74029",
    "description": "Inform Amazon ECR that the image layer upload for a specified registry, repository name, and upload ID, has completed.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Layer Availability",
      "item": [
        {
          "id": "2550bb5a-8925-44b0-add4-12f26a153a5d",
          "name": "batchCheckLayerAvailability",
          "request": {
            "url": "http://example.com/api/?Action=BatchCheckLayerAvailability?layerDigests=layerDigests&registryId=registryId&repositoryName=repositoryName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Check the availability of multiple image layers in a specified registry and repository."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c471686-fd40-4f00-873c-7c939785d9f1"
            }
          ]
        }
      ]
    },
    {
      "name": "Image",
      "item": [
        {
          "id": "f65b8cb8-087e-4d04-a1f4-f83939222392",
          "name": "batchDeleteImage",
          "request": {
            "url": "http://example.com/api/?Action=BatchDeleteImage?imageIds=imageIds&registryId=registryId&repositoryName=repositoryName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a list of specified images within a specified repository."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b008d18-8064-436c-8d59-c1d652694669"
            }
          ]
        },
        {
          "id": "84b0cb75-91ea-4f9c-912a-8e9a1a94ca5b",
          "name": "batchGetImage",
          "request": {
            "url": "http://example.com/api/?Action=BatchGetImage?acceptedMediaTypes=acceptedMediaTypes&imageIds=imageIds&registryId=registryId&repositoryName=repositoryName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets detailed information for specified images within a specified repository."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b713527-187e-4450-9998-f0373daa5db4"
            }
          ]
        }
      ]
    },
    {
      "name": "Layer Upload",
      "item": [
        {
          "id": "203f2e41-9c0e-4799-8da0-9092bcc656d9",
          "name": "completeLayerUpload",
          "request": {
            "url": "http://example.com/api/?Action=CompleteLayerUpload",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Inform Amazon ECR that the image layer upload for a specified registry, repository name, and upload ID, has completed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00ac367c-b56c-44c6-b815-f5678758ce67"
            }
          ]
        }
      ]
    }
  ]
}