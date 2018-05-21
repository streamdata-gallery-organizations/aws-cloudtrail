{
  "info": {
    "name": "AWS CloudTrail API Get Event Selectors",
    "_postman_id": "4971769f-3904-47fd-a5c5-959b99fd586d",
    "description": "Describes the settings for the event selectors that you configured for your trail.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "df2acfcb-bd42-4e72-ba54-c85167e7a29d",
          "name": "AddTags",
          "request": {
            "url": "http://example.com/api/?Action=AddTags?ResourceId=ResourceId&TagsList=TagsList",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds one or more tags to a trail, up to a limit of 50."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89827911-7101-4cb6-be46-1c2370dfed3f"
            }
          ]
        }
      ]
    },
    {
      "name": "Trails",
      "item": [
        {
          "id": "3e8a7705-a41f-40c9-a01d-e436ba85490e",
          "name": "CreateTrail",
          "request": {
            "url": "http://example.com/api/?Action=CreateTrail?CloudWatchLogsLogGroupArn=CloudWatchLogsLogGroupArn&CloudWatchLogsRoleArn=CloudWatchLogsRoleArn&EnableLogFileValidation=EnableLogFileValidation&IncludeGlobalServiceEvents=IncludeGlobalServiceEvents&IsMultiRegionTrail=IsMultiRegionTrail&KmsKeyId=KmsKeyId&Name=Name&S3BucketName=S3BucketName&S3KeyPrefix=S3KeyPrefix&SnsTopicName=SnsTopicName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a trail that specifies the settings for delivery of log data to an Amazon S3 bucket."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6ead3e6-eec9-407e-9548-9b8625727e5a"
            }
          ]
        },
        {
          "id": "d6aae89a-a843-4b9e-a354-19b93506998b",
          "name": "DeleteTrail",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTrail?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a trail."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aacb0902-8557-42a3-a118-5c760d5b0025"
            }
          ]
        },
        {
          "id": "8a312166-9692-418c-8c2f-d31f023e3f75",
          "name": "DescribeTrails",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTrails?includeShadowTrails=includeShadowTrails&trailNameList=trailNameList",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves settings for the trail associated with the current region for your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "734c48d2-185b-4583-9287-ac78df04eec0"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Selectors",
      "item": [
        {
          "id": "60969716-2eb2-4e4f-a6bf-506e8af23016",
          "name": "GetEventSelectors",
          "request": {
            "url": "http://example.com/api/?Action=GetEventSelectors?TrailName=TrailName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the settings for the event selectors that you configured for your trail."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23177d8a-096e-4054-8750-1e9025d56073"
            }
          ]
        }
      ]
    }
  ]
}