{
  "info": {
    "name": "Amazon EC2 Systems Manager API Describe Instance Information",
    "_postman_id": "c66547d1-9839-48b6-8736-551eb942b2db",
    "description": "Describes one or more of your instances.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "1c4ad995-8251-433b-bd7c-2a61de4ab121",
          "name": "addTagsToResource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceId=ResourceId&ResourceType=ResourceType&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or overwrites one or more tags for the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7900116a-f8ba-481c-8c8e-8f2eeea5426b"
            }
          ]
        }
      ]
    },
    {
      "name": "Cancel",
      "item": [
        {
          "id": "88a31d23-0d5a-4840-b8a3-cd39b35f040c",
          "name": "cancelCommand",
          "request": {
            "url": "http://example.com/api/?Action=CancelCommand?CommandId=CommandId&InstanceIds=InstanceIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attempts to cancel the command specified by the Command ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df7e50f7-1e08-4583-a5aa-5f85bcb1991a"
            }
          ]
        }
      ]
    },
    {
      "name": "Activation",
      "item": [
        {
          "id": "b31fa896-3c73-4557-b96c-4d8524357ff3",
          "name": "createActivation",
          "request": {
            "url": "http://example.com/api/?Action=CreateActivation?DefaultInstanceName=DefaultInstanceName&Description=Description&ExpirationDate=ExpirationDate&IamRole=IamRole&RegistrationLimit=RegistrationLimit",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers your on-premises server or virtual machine with Amazon EC2 so that you can manage\n   these resources using Run Command."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d10bd21-de98-4dfd-9deb-34abdab00d32"
            }
          ]
        },
        {
          "id": "e978dc35-3db0-48e4-8f87-595cb16c4789",
          "name": "deleteActivation",
          "request": {
            "url": "http://example.com/api/?Action=DeleteActivation?ActivationId=ActivationId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an activation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d461cc82-004c-4f38-a547-c1d23f27d4dd"
            }
          ]
        }
      ]
    },
    {
      "name": "Association",
      "item": [
        {
          "id": "8ff020ff-ebd6-4170-bf13-5acf6b998a2e",
          "name": "createAssociation",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssociation?DocumentVersion=DocumentVersion&InstanceId=InstanceId&Name=Name&OutputLocation=OutputLocation&Parameters=Parameters&ScheduleExpression=ScheduleExpression&Targets=Targets",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates the specified SSM document with the specified instances or targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51cdb106-3998-4c68-a8fd-d3836d8ceb7c"
            }
          ]
        },
        {
          "id": "b7bfdf3c-18f7-4652-b02d-31e617522469",
          "name": "createAssociationBatch",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssociationBatch?Entries=Entries",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates the specified SSM document with the specified instances or targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "780f22f9-9e4a-4c65-b937-e4f950b77d22"
            }
          ]
        },
        {
          "id": "32df1fed-5050-41ca-b618-6693f379fba6",
          "name": "deleteAssociation",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAssociation?AssociationId=AssociationId&InstanceId=InstanceId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disassociates the specified SSM document from the specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbb71e03-2440-45f3-9274-45d87917e71d"
            }
          ]
        },
        {
          "id": "7a2ed59e-1308-4326-9679-62df4bf3ffb3",
          "name": "describeAssociation",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAssociation?AssociationId=AssociationId&InstanceId=InstanceId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the associations for the specified SSM document or instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a00ebdd4-3865-45f4-9c43-8c5af2a16f40"
            }
          ]
        }
      ]
    },
    {
      "name": "Document",
      "item": [
        {
          "id": "6e7e3622-0d5b-405d-86d4-495be625963e",
          "name": "createDocument",
          "request": {
            "url": "http://example.com/api/?Action=CreateDocument?Content=Content&DocumentType=DocumentType&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f9b5e4d-f119-4726-a62a-8fc45678dff8"
            }
          ]
        },
        {
          "id": "6b5795fe-c5ad-4d3e-b7ac-ad806ba10df5",
          "name": "deleteDocument",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDocument?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the SSM document and all instance associations to the document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1089bf0-e4e7-4897-95cc-797ef406a570"
            }
          ]
        },
        {
          "id": "e8c8d17c-88b5-4a93-88ba-3c6cfc8286af",
          "name": "describeDocument",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDocument?DocumentVersion=DocumentVersion&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6848c606-670a-4cda-8027-f7e7ed10ebf3"
            }
          ]
        },
        {
          "id": "ea5728c2-a144-4101-82f5-9f8ea21541b3",
          "name": "describeDocumentPermission",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDocumentPermission?Name=Name&PermissionType=PermissionType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the permissions for an SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f4fbe30-78e3-4999-ae49-512168b77bd2"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance",
      "item": [
        {
          "id": "1dd47756-0040-4c11-948d-694f4dbdf5ef",
          "name": "createMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=CreateMaintenanceWindow?AllowUnassociatedTargets=AllowUnassociatedTargets&ClientToken=ClientToken&Cutoff=Cutoff&Duration=Duration&Name=Name&Schedule=Schedule",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79f78a8a-5d4e-4b9c-b42d-bfdbecfb0736"
            }
          ]
        },
        {
          "id": "ba9c88f4-bbae-411a-8c34-8f3c11bea1a6",
          "name": "deleteMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeleteMaintenanceWindow?WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea7266db-d22f-4cce-8e97-4c6816a021ef"
            }
          ]
        }
      ]
    },
    {
      "name": "Baseline",
      "item": [
        {
          "id": "7043879a-bde4-4b11-8fb4-6c7190d9c718",
          "name": "createPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=CreatePatchBaseline?ApprovalRules=ApprovalRules&ApprovedPatches=ApprovedPatches&ClientToken=ClientToken&Description=Description&GlobalFilters=GlobalFilters&Name=Name&RejectedPatches=RejectedPatches",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9ccdd37-7e39-46cb-a8d1-f48bcf747b68"
            }
          ]
        },
        {
          "id": "d7f960d4-293b-4d8f-bdf7-1118da722249",
          "name": "deletePatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=DeletePatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11e83338-6141-4d3b-957f-bb8d8920336d"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameter",
      "item": [
        {
          "id": "4b1ceafd-1c4f-4584-8f3c-f0c22805403a",
          "name": "deleteParameter",
          "request": {
            "url": "http://example.com/api/?Action=DeleteParameter?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a parameter from the system."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e79c4a7f-7511-415a-8027-0b25cac9eed1"
            }
          ]
        }
      ]
    },
    {
      "name": "Deregister",
      "item": [
        {
          "id": "27812409-e95b-4aea-8bf2-83b631aec3ec",
          "name": "deregisterManagedInstance",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterManagedInstance?InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the server or virtual machine from the list of registered servers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2142597-9de9-49a5-a556-0b254c960f1b"
            }
          ]
        },
        {
          "id": "1fcd5fd5-7585-4ab7-8637-9aa1e3212cad",
          "name": "deregisterPatchBaselineForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterPatchBaselineForPatchGroup?BaselineId=BaselineId&PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a patch group from a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3dbda70c-f8fe-4879-9b09-0c49bfd009b3"
            }
          ]
        },
        {
          "id": "5845cc0b-bedc-4eea-ae4e-a6fcfff9b28f",
          "name": "deregisterTargetFromMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTargetFromMaintenanceWindow?WindowId=WindowId&WindowTargetId=WindowTargetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a target from a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b2f8228-d5f4-4ba7-aa27-0ab7e094fe8f"
            }
          ]
        },
        {
          "id": "9db2e640-8361-4dc6-af3d-8688cc16aa64",
          "name": "deregisterTaskFromMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTaskFromMaintenanceWindow?WindowId=WindowId&WindowTaskId=WindowTaskId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a task from a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27075065-219b-460e-bb13-d70e24baf2f3"
            }
          ]
        }
      ]
    },
    {
      "name": "Activations",
      "item": [
        {
          "id": "733ab9cb-5a14-4394-a522-085083685a9c",
          "name": "describeActivations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeActivations?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Details about the activation, including: the date and time the activation was created,\n   the expiration date, the IAM role assigned to the instances in the activation, and the number of\n   instances activated by this registration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b02461ee-b962-4163-aee4-e125fba1deb5"
            }
          ]
        }
      ]
    },
    {
      "name": "Automation",
      "item": [
        {
          "id": "99bda17e-a307-4fb8-9c49-d3244dea638f",
          "name": "describeAutomationExecutions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAutomationExecutions?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides details about all active and terminated Automation executions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e8bdf44-905b-431d-93da-e01517c55a5f"
            }
          ]
        }
      ]
    },
    {
      "name": "Available",
      "item": [
        {
          "id": "a3dfe927-f4e1-4ea2-9299-6f5233288178",
          "name": "describeAvailablePatches",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAvailablePatches?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all patches that could possibly be included in a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a3f0904-fcab-4a71-babe-1ba21af63901"
            }
          ]
        }
      ]
    },
    {
      "name": "Effective",
      "item": [
        {
          "id": "0ab74bcf-1207-4292-b01f-84628f4a333a",
          "name": "describeEffectiveInstanceAssociations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEffectiveInstanceAssociations?InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All associations for the instance(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d78c74c-c551-4cfc-b188-3f9ad0a0e9dc"
            }
          ]
        },
        {
          "id": "2960cdee-ae92-4e38-a341-1128d8969d0d",
          "name": "describeEffectivePatchesForPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEffectivePatchesForPatchBaseline?BaselineId=BaselineId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the current effective patches (the patch and the approval state) for the specified patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6bc3a60f-dfa4-4f3f-afbb-2775e9302cd3"
            }
          ]
        }
      ]
    },
    {
      "name": "Instance",
      "item": [
        {
          "id": "9e6065a9-3f65-49ad-9227-1dd98a2b0168",
          "name": "describeInstanceAssociationsStatus",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstanceAssociationsStatus?InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The status of the associations for the instance(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b16d220-40aa-4ac5-ae5f-5b85bb1e60b6"
            }
          ]
        },
        {
          "id": "3bef8f9d-d306-4b7a-b6dd-77c62b1d59e3",
          "name": "describeInstanceInformation",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstanceInformation?Filters=Filters&InstanceInformationFilterList=InstanceInformationFilterList&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more of your instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e4d845b5-a153-48dc-8f95-5ad546b35455"
            }
          ]
        }
      ]
    }
  ]
}