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
  /book:
    get:
      summary: List books.
      description: List the books, 20 per page.
      operationId: list-the-books-20-per-page
      x-api-path-slug: book-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the books
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Books
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
  /book/{book_identifier}:
    get:
      summary: Get a representation of a book.
      description: Get JSON which represents the structure of a book.
      operationId: get-json-which-represents-the-structure-of-a-book
      x-api-path-slug: bookbook-identifier-get
      parameters:
      - in: path
        name: book_identifier
        description: book_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the book
      - in: query
        name: with_regions
        description: Include regions associated with the book
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Book
---