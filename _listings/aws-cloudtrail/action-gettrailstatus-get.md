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
  /?Action=GetTrailStatus:
    get:
      summary: Get Trail Status
      description: Returns a JSON-formatted list of information about the specified
        trail
      operationId: GetTrailStatus
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