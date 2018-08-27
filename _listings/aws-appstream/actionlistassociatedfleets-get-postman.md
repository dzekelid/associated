{
  "info": {
    "name": "AWS AppStream 2.0 API List Associated Fleets",
    "_postman_id": "cb76ec56-1e1c-4e87-9b79-7d0c561cc8fe",
    "description": "Lists all fleets associated with the stack.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Fleet",
      "item": [
        {
          "id": "42901b9e-b738-49e3-80cf-35d65955c134",
          "name": "AssociateFleet",
          "request": {
            "url": "http://example.com/api/?Action=AssociateFleet?FleetName=FleetName&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associate a fleet to a stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb58bb8a-04fa-4371-ac6d-d2c67498428e"
            }
          ]
        },
        {
          "id": "cb4cd925-9c6a-4d25-91fa-fbab0ab1d048",
          "name": "CreateFleet",
          "request": {
            "url": "http://example.com/api/?Action=CreateFleet?ComputeCapacity=ComputeCapacity&Description=Description&DisconnectTimeoutInSeconds=DisconnectTimeoutInSeconds&DisplayName=DisplayName&ImageName=ImageName&InstanceType=InstanceType&MaxUserDurationInSeconds=MaxUserDurationInSeconds&Name=Name&VpcConfig=VpcConfig",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new fleet."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab54f52a-9360-4851-bb75-a44eb12683cb"
            }
          ]
        },
        {
          "id": "dd2cb6d0-0156-486d-be03-ca031a24cb3e",
          "name": "CreateStack",
          "request": {
            "url": "http://example.com/api/?Action=CreateStack?Description=Description&DisplayName=DisplayName&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1422a1c7-10c6-45aa-a57b-b4b32e86a7fc"
            }
          ]
        },
        {
          "id": "e1da809f-e2a8-43f5-901c-d0311c9af591",
          "name": "DeleteFleet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteFleet?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a fleet."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7bcb8539-a481-403f-889a-b37b470e1da4"
            }
          ]
        },
        {
          "id": "3312a0f4-57f2-4844-a39f-2d39e6b2ac56",
          "name": "DescribeFleets",
          "request": {
            "url": "http://example.com/api/?Action=DescribeFleets?Names=Names&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "If fleet names are provided, this operation describes the specified fleets;\n            otherwise, all the fleets in the account are described."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "19f8f5b0-905a-438b-b342-1c1d006885f6"
            }
          ]
        },
        {
          "id": "74a46e38-d54b-4114-89c0-73dc37f4a9a0",
          "name": "DisassociateFleet",
          "request": {
            "url": "http://example.com/api/?Action=DisassociateFleet?FleetName=FleetName&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disassociates a fleet from a stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "004a086e-cb0d-492f-afa1-127e8ff4f9a0"
            }
          ]
        },
        {
          "id": "36feacf1-e2fc-45da-a2ac-82a36df36210",
          "name": "ListAssociatedFleets",
          "request": {
            "url": "http://example.com/api/?Action=ListAssociatedFleets?NextToken=NextToken&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all fleets associated with the stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0000089e-a310-4a13-ab4c-83ad6bedadbf"
            }
          ]
        }
      ]
    },
    {
      "name": "URL",
      "item": [
        {
          "id": "278d175e-ebea-4ea9-b38d-9436fceb1b32",
          "name": "CreateStreamingURL",
          "request": {
            "url": "http://example.com/api/?Action=CreateStreamingURL?ApplicationId=ApplicationId&FleetName=FleetName&SessionContext=SessionContext&StackName=StackName&UserId=UserId&Validity=Validity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a URL to start an AppStream 2."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86e4443c-4345-4dcf-9538-92a5b945b774"
            }
          ]
        }
      ]
    },
    {
      "name": "Stack",
      "item": [
        {
          "id": "adbb6adf-378e-4c03-bed0-9515cf3a3ba0",
          "name": "DeleteStack",
          "request": {
            "url": "http://example.com/api/?Action=DeleteStack?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54a293cb-d1e1-4255-ba41-19c1f9558c36"
            }
          ]
        }
      ]
    },
    {
      "name": "Images",
      "item": [
        {
          "id": "c761fc46-c62f-44eb-bc5f-5c5be5a7f709",
          "name": "DescribeImages",
          "request": {
            "url": "http://example.com/api/?Action=DescribeImages?Names=Names",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the images."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8e0399f-3edb-4b68-bdc3-ed5862bc004d"
            }
          ]
        }
      ]
    },
    {
      "name": "Sessions",
      "item": [
        {
          "id": "86be5752-a682-4f39-a58e-17b65306142b",
          "name": "DescribeSessions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSessions?FleetName=FleetName&Limit=Limit&NextToken=NextToken&StackName=StackName&UserId=UserId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the streaming sessions for a stack and a fleet."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "434f88cd-bf04-4b4d-bc3b-b9c63a37a835"
            }
          ]
        }
      ]
    },
    {
      "name": "Stacks",
      "item": [
        {
          "id": "dacfb19d-84d8-41f4-b229-42889aa41609",
          "name": "DescribeStacks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStacks?Names=Names&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "If stack names are not provided, this operation describes the specified stacks;\n            otherwise, all stacks in the account are described."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f519b1ce-8a11-41a4-8e09-bfc13408619c"
            }
          ]
        }
      ]
    },
    {
      "name": "Session",
      "item": [
        {
          "id": "201fd534-551e-4cfe-bf2b-977ba3759168",
          "name": "ExpireSession",
          "request": {
            "url": "http://example.com/api/?Action=ExpireSession?SessionId=SessionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This operation immediately stops a streaming session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43301988-5e65-47bd-9298-a6af5a6586a2"
            }
          ]
        }
      ]
    }
  ]
}