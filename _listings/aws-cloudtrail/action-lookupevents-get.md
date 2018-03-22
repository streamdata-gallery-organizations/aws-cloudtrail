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
  /?Action=LookupEvents:
    get:
      summary: Lookup Events
      description: |-
        Looks up API activity events captured by CloudTrail that create, update, or delete
                 resources in your account
      operationId: LookupEvents
      parameters:
      - in: query
        name: EndTime
        description: Specifies that only events that occur before or at the specified
          time are returned
        type: string
      - in: query
        name: LookupAttributes
        description: Contains a list of lookup attributes
        type: string
      - in: query
        name: MaxResults
        description: The number of events to return
        type: string
      - in: query
        name: NextToken
        description: The token to use to get the next page of results after a previous
          API call
        type: string
      - in: query
        name: StartTime
        description: Specifies that only events that occur after or at the specified
          time are returned
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