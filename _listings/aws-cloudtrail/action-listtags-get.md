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
  /?Action=ListTags&k=1:
    get:
      summary: List Tags
      description: Lists the tags for the trail in the current region
      operationId: ListTags
      parameters:
      - in: query
        name: NextToken
        description: Reserved for future use
        type: string
      - in: query
        name: ResourceIdList
        description: Specifies a list of trail ARNs whose tags will be listed
        type: string
      responses:
        200:
          description: OK
      tags:
      - service access policies
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