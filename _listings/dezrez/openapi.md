---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/property/bookvaluation:
    post:
      summary: A command driven endpoint to Book a Valuation.
      description: A command driven endpoint to book a valuation..
      operationId: Property_BookValuationBybookValuationData
      x-api-path-slug: apipropertybookvaluation-post
      parameters:
      - in: body
        name: bookValuationData
        description: A wrapper for the various data contracts needed
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - A
      - Command
      - Driven
      - Endpoint
      - To
      - Book
      - Valuation
  /api/viewing/bookviewing:
    post:
      summary: Book a Viewing.
      description: Book a viewing..
      operationId: Viewing_BookViewingBybookViewingDataContract
      x-api-path-slug: apiviewingbookviewing-post
      parameters:
      - in: body
        name: bookViewingDataContract
        description: the viewing detail
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Book
      - Viewing
  /api/viewing/bookmultiviewing:
    post:
      summary: Book multiple viewings appointment
      description: Book multiple viewings appointment.
      operationId: Viewing_BookMultiViewingBydataContract
      x-api-path-slug: apiviewingbookmultiviewing-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Book
      - Multiple
      - Viewings
      - Appointment
---