swagger: "2.0"
x-collection-name: Google Books
x-complete: 1
info:
  title: Books
  description: searches-for-books-and-manages-your-google-books-library-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /books/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /volumes/{volumeId}/associated:
    get:
      summary: Get Associated
      description: Return a list of associated books.
      operationId: books.volumes.associated.list
      x-api-path-slug: volumesvolumeidassociated-get
      parameters:
      - in: query
        name: association
        description: Association type
      - in: query
        name: locale
        description: ISO-639-1 language and ISO-3166-1 country code
      - in: query
        name: maxAllowedMaturityRating
        description: The maximum allowed maturity rating of returned recommendations
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: path
        name: volumeId
        description: ID of the source volume
      responses:
        200:
          description: OK
      tags:
      - Associated