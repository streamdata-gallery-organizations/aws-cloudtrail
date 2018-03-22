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
  /?Action=GetEventSelectors:
    get:
      summary: Get Event Selectors
      description: Describes the settings for the event selectors that you configured
        for your trail
      operationId: GetEventSelectors
      parameters:
      - in: query
        name: TrailName
        description: Specifies the name of the trail or trail ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - event selectors
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