---
swagger: "2.0"
info:
  title: AWS CloudTrail API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateTrail&k=1:
    get:
      summary: Create Trail
      description: Creates a trail that specifies the settings for delivery of log
        data to an Amazon S3 bucket
      operationId: CreateTrail
      parameters:
      - in: query
        name: CloudWatchLogsLogGroupArn
        description: Specifies a log group name using an Amazon Resource Name (ARN),
          a unique identifier that represents the log group to which CloudTrail logs
          will be delivered
        type: string
      - in: query
        name: CloudWatchLogsRoleArn
        description: Specifies the role for the CloudWatch Logs endpoint to assume
          to write to a user's log group
        type: string
      - in: query
        name: EnableLogFileValidation
        description: Specifies whether log file integrity validation is enabled
        type: string
      - in: query
        name: IncludeGlobalServiceEvents
        description: Specifies whether the trail is publishing events from global
          services such as IAM to the log files
        type: string
      - in: query
        name: IsMultiRegionTrail
        description: Specifies whether the trail is created in the current region
          or in all regions
        type: string
      - in: query
        name: KmsKeyId
        description: Specifies the KMS key ID to use to encrypt the logs delivered
          by CloudTrail
        type: string
      - in: query
        name: Name
        description: Specifies the name of the trail
        type: string
      - in: query
        name: S3BucketName
        description: Specifies the name of the Amazon S3 bucket designated for publishing
          log files
        type: string
      - in: query
        name: S3KeyPrefix
        description: Specifies the Amazon S3 key prefix that comes after the name
          of the bucket you have designated         for log file delivery
        type: string
      - in: query
        name: SnsTopicName
        description: Specifies the name of the Amazon SNS topic defined for notification
          of log file delivery
        type: string
      responses:
        200:
          description: OK
      tags:
      - trails
definitions: []
x-collection-name: AWS CloudTrail
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