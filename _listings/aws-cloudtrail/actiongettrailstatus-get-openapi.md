---
swagger: "2.0"
x-collection-name: AWS CloudTrail
x-complete: 0
info:
  title: AWS CloudTrail API Get Trail Status
  version: 1.0.0
  description: Returns a JSON-formatted list of information about the specified trail.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddTags:
    get:
      summary: Add Tags
      description: Adds one or more tags to a trail, up to a limit of 50.
      operationId: AddTags
      x-api-path-slug: actionaddtags-get
      parameters:
      - in: query
        name: ResourceId
        description: Specifies the ARN of the trail to which one or more tags will
          be added
        type: string
      - in: query
        name: TagsList
        description: Contains a list of CloudTrail tags, up to a limit of 50
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=CreateTrail:
    get:
      summary: Create Trail
      description: Creates a trail that specifies the settings for delivery of log
        data to an Amazon S3 bucket.
      operationId: CreateTrail
      x-api-path-slug: actioncreatetrail-get
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
          to write to a users log group
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
      - Trails
  /?Action=DeleteTrail:
    get:
      summary: Delete Trail
      description: Deletes a trail.
      operationId: DeleteTrail
      x-api-path-slug: actiondeletetrail-get
      parameters:
      - in: query
        name: Name
        description: Specifies the name or the CloudTrail ARN of the trail to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Trails
  /?Action=DescribeTrails:
    get:
      summary: Describe Trails
      description: Retrieves settings for the trail associated with the current region
        for your account.
      operationId: DescribeTrails
      x-api-path-slug: actiondescribetrails-get
      parameters:
      - in: query
        name: includeShadowTrails
        description: Specifies whether to include shadow trails in the response
        type: string
      - in: query
        name: trailNameList
        description: Specifies a list of trail names, trail ARNs, or both, of the
          trails to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Trails
  /?Action=GetEventSelectors:
    get:
      summary: Get Event Selectors
      description: Describes the settings for the event selectors that you configured
        for your trail.
      operationId: GetEventSelectors
      x-api-path-slug: actiongeteventselectors-get
      parameters:
      - in: query
        name: TrailName
        description: Specifies the name of the trail or trail ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Selectors
  /?Action=GetTrailStatus:
    get:
      summary: Get Trail Status
      description: Returns a JSON-formatted list of information about the specified
        trail.
      operationId: GetTrailStatus
      x-api-path-slug: actiongettrailstatus-get
      parameters:
      - in: query
        name: Name
        description: Specifies the name or the CloudTrail ARN of the trail for which
          you are requesting status
        type: string
      responses:
        200:
          description: OK
      tags:
      - Trails
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