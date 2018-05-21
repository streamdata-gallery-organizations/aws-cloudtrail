---
swagger: "2.0"
x-collection-name: AWS CloudTrail
x-complete: 0
info:
  title: AWS CloudTrail API Add Tags
  version: 1.0.0
  description: Adds one or more tags to a trail, up to a limit of 50.
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