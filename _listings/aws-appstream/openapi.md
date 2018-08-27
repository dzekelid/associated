swagger: "2.0"
x-collection-name: AWS AppStream
x-complete: 1
info:
  title: AWS AppStream 2.0 API
  description: amazon-appstream-2-0-is-a-fully-managed-secure-application-streaming-service-that-allows-you-to-stream-desktop-applications-from-aws-to-any-device-running-a-web-browser-without-rewriting-them--amazon-appstream-2-0-provides-users-instanton-access-to-the-applications-they-need-and-a-responsive-fluid-user-experience-on-the-device-of-their-choice-
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
  /?Action=ListAssociatedStacks:
    get:
      summary: List Associated Stacks
      description: Lists all stacks to which the specified fleet is associated.
      operationId: ListAssociatedStacks
      x-api-path-slug: actionlistassociatedstacks-get
      parameters:
      - in: query
        name: FleetName
        description: The name of the fleet whose associated stacks are listed
        type: string
      - in: query
        name: NextToken
        description: The pagination token to use to retrieve the next page of results
          for this operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack