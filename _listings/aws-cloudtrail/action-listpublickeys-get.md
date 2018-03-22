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
  /?Action=ListPublicKeys:
    get:
      summary: List Public Keys
      description: Returns all public keys whose private keys were used to sign the
        digest files within the specified time range
      operationId: ListPublicKeys
      parameters:
      - in: query
        name: EndTime
        description: Optionally specifies, in UTC, the end of the time range to look
          up public keys for CloudTrail digest files
        type: string
      - in: query
        name: NextToken
        description: Reserved for future use
        type: string
      - in: query
        name: StartTime
        description: Optionally specifies, in UTC, the start of the time range to
          look up public keys for CloudTrail digest files
        type: string
      responses:
        200:
          description: OK
      tags:
      - public keys
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