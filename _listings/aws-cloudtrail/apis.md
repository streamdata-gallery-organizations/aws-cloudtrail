---
name: AWS CloudTrail
x-slug: aws-cloudtrail
description: AWS CloudTrail is a web service that records AWS API calls for your account
  and delivers log files to you. The recorded information includes the identity of
  the API caller, the time of the API call, the source IP address of the API caller,
  the request parameters, and the response elements returned by the AWS service.With
  CloudTrail, you can get a history of AWS API calls for your account, including API
  calls made via the AWS Management Console, AWS SDKs, command line tools, and higher-level
  AWS services (such as AWS CloudFormation). The AWS API call history produced by
  CloudTrail enables security analysis, resource change tracking, and compliance auditing.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudTrail.png
x-kinRank: "10"
x-alexaRank: ""
tags: AWS CloudTrail
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudtrail/master/_listings/aws-cloudtrail/apis.md
specificationVersion: "0.14"
apis:
- name: AWS CloudTrail API Add Tags
  x-api-slug: aws-cloudtrail-api
  description: Adds one or more tags to a trail, up to a limit of 50.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudTrail.png
  humanURL: https://aws.amazon.com/cloudtrail/
  baseURL: ://///?Action=AddTags
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudtrail/master/_listings/aws-cloudtrail/actionaddtags-get-openapi.md
- name: AWS CloudTrail API Create Trail
  x-api-slug: aws-cloudtrail-api
  description: Creates a trail that specifies the settings for delivery of log data
    to an Amazon S3 bucket.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudTrail.png
  humanURL: https://aws.amazon.com/cloudtrail/
  baseURL: ://///?Action=CreateTrail
  tags: Trails
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudtrail/master/_listings/aws-cloudtrail/actioncreatetrail-get-openapi.md
- name: AWS CloudTrail API Delete Trail
  x-api-slug: aws-cloudtrail-api
  description: Deletes a trail.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudTrail.png
  humanURL: https://aws.amazon.com/cloudtrail/
  baseURL: ://///?Action=DeleteTrail
  tags: Trails
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudtrail/master/_listings/aws-cloudtrail/actiondeletetrail-get-openapi.md
- name: AWS CloudTrail API Describe Trails
  x-api-slug: aws-cloudtrail-api
  description: Retrieves settings for the trail associated with the current region
    for your account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudTrail.png
  humanURL: https://aws.amazon.com/cloudtrail/
  baseURL: ://///?Action=DescribeTrails
  tags: Trails
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudtrail/master/_listings/aws-cloudtrail/actiondescribetrails-get-openapi.md
- name: AWS CloudTrail API Get Event Selectors
  x-api-slug: aws-cloudtrail-api
  description: Describes the settings for the event selectors that you configured
    for your trail.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudTrail.png
  humanURL: https://aws.amazon.com/cloudtrail/
  baseURL: ://///?Action=GetEventSelectors
  tags: Event Selectors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudtrail/master/_listings/aws-cloudtrail/actiongeteventselectors-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudtrail/master/_listings/aws-cloudtrail/actiongeteventselectors-get-openapi.md
- name: AWS CloudTrail API Get Trail Status
  x-api-slug: aws-cloudtrail-api
  description: Returns a JSON-formatted list of information about the specified trail.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudTrail.png
  humanURL: https://aws.amazon.com/cloudtrail/
  baseURL: ://///?Action=GetTrailStatus
  tags: Trails
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudtrail/master/_listings/aws-cloudtrail/actiongettrailstatus-get-openapi.md
- name: AWS CloudTrail API List Public Keys
  x-api-slug: aws-cloudtrail-api
  description: Returns all public keys whose private keys were used to sign the digest
    files within the specified time range.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudTrail.png
  humanURL: https://aws.amazon.com/cloudtrail/
  baseURL: ://///?Action=ListPublicKeys
  tags: Public Keys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudtrail/master/_listings/aws-cloudtrail/actionlistpublickeys-get-openapi.md
- name: AWS CloudTrail API List Tags
  x-api-slug: aws-cloudtrail-api
  description: Lists the tags for the trail in the current region.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudTrail.png
  humanURL: https://aws.amazon.com/cloudtrail/
  baseURL: ://///?Action=ListTags
  tags: Service Access Policies
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudtrail/master/_listings/aws-cloudtrail/actionlisttags-get-openapi.md
- name: AWS CloudTrail API Lookup Events
  x-api-slug: aws-cloudtrail-api
  description: |-
    Looks up API activity events captured by CloudTrail that create, update, or delete
             resources in your account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudTrail.png
  humanURL: https://aws.amazon.com/cloudtrail/
  baseURL: ://///?Action=LookupEvents
  tags: Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudtrail/master/_listings/aws-cloudtrail/actionlookupevents-get-openapi.md
- name: AWS CloudTrail API Put Event Selectors
  x-api-slug: aws-cloudtrail-api
  description: Configures an event selector for your trail.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudTrail.png
  humanURL: https://aws.amazon.com/cloudtrail/
  baseURL: ://///?Action=PutEventSelectors
  tags: Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudtrail/master/_listings/aws-cloudtrail/actionputeventselectors-get-openapi.md
- name: AWS CloudTrail API Remove Tags
  x-api-slug: aws-cloudtrail-api
  description: Removes the specified tags from a trail.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudTrail.png
  humanURL: https://aws.amazon.com/cloudtrail/
  baseURL: ://///?Action=RemoveTags
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudtrail/master/_listings/aws-cloudtrail/actionremovetags-get-openapi.md
- name: AWS CloudTrail API Start Logging
  x-api-slug: aws-cloudtrail-api
  description: Starts the recording of AWS API calls and log file delivery for a trail.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudTrail.png
  humanURL: https://aws.amazon.com/cloudtrail/
  baseURL: ://///?Action=StartLogging
  tags: Logging
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudtrail/master/_listings/aws-cloudtrail/actionstartlogging-get-openapi.md
- name: AWS CloudTrail API Stop Logging
  x-api-slug: aws-cloudtrail-api
  description: Suspends the recording of AWS API calls and log file delivery for the
    specified trail.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudTrail.png
  humanURL: https://aws.amazon.com/cloudtrail/
  baseURL: ://///?Action=StopLogging
  tags: Logging
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudtrail/master/_listings/aws-cloudtrail/actionstoplogging-get-openapi.md
- name: AWS CloudTrail API Update Trail
  x-api-slug: aws-cloudtrail-api
  description: Updates the settings that specify delivery of log files.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudTrail.png
  humanURL: https://aws.amazon.com/cloudtrail/
  baseURL: ://///?Action=UpdateTrail
  tags: Trails
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudtrail/master/_listings/aws-cloudtrail/actionupdatetrail-get-openapi.md
- name: AWS CloudTrail API
  x-api-slug: aws-cloudtrail-api
  description: AWS CloudTrail is a web service that records AWS API calls for your
    account and delivers log files to you. The recorded information includes the identity
    of the API caller, the time of the API call, the source IP address of the API
    caller, the request parameters, and the response elements returned by the AWS
    service.With CloudTrail, you can get a history of AWS API calls for your account,
    including API calls made via the AWS Management Console, AWS SDKs, command line
    tools, and higher-level AWS services (such as AWS CloudFormation). The AWS API
    call history produced by CloudTrail enables security analysis, resource change
    tracking, and compliance auditing.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSCloudTrail.png
  humanURL: https://aws.amazon.com/cloudtrail/
  baseURL: :///
  tags: AWS CloudTrail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-cloudtrail/master/_listings/aws-cloudtrail/openapi.md
x-common:
- type: x-console
  url: https://console.aws.amazon.com/cloudtrail/home
- type: x-documentation
  url: http://docs.aws.amazon.com/awscloudtrail/latest/APIReference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/cloudtrail/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=168
- type: x-getting-started
  url: https://aws.amazon.com/cloudtrail/getting-started/
- type: x-partners
  url: https://aws.amazon.com/cloudtrail/partners/
- type: x-pricing
  url: https://aws.amazon.com/cloudtrail/pricing/
- type: x-website
  url: https://aws.amazon.com/cloudtrail/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---