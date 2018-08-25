---
swagger: "2.0"
x-collection-name: AWS AppStream
x-complete: 0
info:
  title: AWS AppStream 2.0 API List Associated Fleets
  description: Lists all fleets associated with the stack.
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListAssociatedFleets:
    get:
      summary: List Associated Fleets
      description: Lists all fleets associated with the stack.
      operationId: ListAssociatedFleets
      x-api-path-slug: actionlistassociatedfleets-get
      parameters:
      - in: query
        name: NextToken
        description: The pagination token to use to retrieve the next page of results
          for this operation
        type: string
      - in: query
        name: StackName
        description: The name of the stack whose associated fleets are listed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Fleet
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