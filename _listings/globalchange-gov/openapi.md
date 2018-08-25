---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 1
info:
  title: Global Change Information System API
  description: who-we-are-what-the-gcis-is-and-how-we-use-identifiers-and-semantic-information-to-provide-points-of-reference-and-traceability--examples-and-tutorials-for-using-this-system-as-a-researcher-citizen-scientist-application-developer-or-information-theorist--a-description-of-how-the-information-is-structured-including-the-overlaps-between-relational-and-semantic-representations-of-the-information--complete-documentation-for-the-api-including-methods-for-browsing-and-finding-resources-
  version: v1
host: data.globalchange.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /report/{report_identifier}/array:
    get:
      summary: List arrays associated with a report.
      description: List the arrays associated with a report, 20 per page.
      operationId: list-the-arrays-associated-with-a-report-20-per-page
      x-api-path-slug: reportreport-identifierarray-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the arrays
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Arrays
      - Associated
      - Report
  /report/{report_identifier}/book:
    get:
      summary: List books associated with a report.
      description: List the books associated with a report, 20 per page.
      operationId: list-the-books-associated-with-a-report-20-per-page
      x-api-path-slug: reportreport-identifierbook-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the books
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Books
      - Associated
      - Report
  /report/{report_identifier}/image:
    get:
      summary: List images associated with a report.
      description: List the images associated with a report, 20 per page.
      operationId: list-the-images-associated-with-a-report-20-per-page
      x-api-path-slug: reportreport-identifierimage-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the images
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Images
      - Associated
      - Report
  /report/{report_identifier}/webpage:
    get:
      summary: List webpages associated with a report.
      description: List the webpages associated with a report, 20 per page.
      operationId: list-the-webpages-associated-with-a-report-20-per-page
      x-api-path-slug: reportreport-identifierwebpage-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the webpages
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Webpages
      - Associated
      - Report
---