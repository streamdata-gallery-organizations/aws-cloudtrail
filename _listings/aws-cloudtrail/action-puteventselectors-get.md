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
  /?Action=PutEventSelectors:
    get:
      summary: Put Event Selectors
      description: Configures an event selector for your trail
      operationId: PutEventSelectors
      parameters:
      - in: query
        name: EventSelectors
        description: Specifies the settings for your event selectors
        type: string
      - in: query
        name: TrailName
        description: Specifies the name of the trail or trail ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - events
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