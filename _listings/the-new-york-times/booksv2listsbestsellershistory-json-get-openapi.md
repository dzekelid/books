---
swagger: "2.0"
x-collection-name: The New York Times
x-complete: 0
info:
  title: The New York Times Best Seller History List
  description: The Best Sellers history service returns books and their history on
    the NYT Best Sellers lists.
  termsOfService: https://developer.nytimes.com/tou
  version: 2.0.0
host: api.nytimes.com
basePath: /svc
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /books/v2/lists/best-sellers/history.json:
    get:
      summary: Best Seller History List
      description: The Best Sellers history service returns books and their history
        on the NYT Best Sellers lists.
      operationId: GET_lists-best-sellers-history-json
      x-api-path-slug: booksv2listsbestsellershistory-json-get
      parameters:
      - in: query
        name: age-group
        description: The target age group for the best seller
      - in: query
        name: author
        description: The author of the best seller
      - in: query
        name: contributor
        description: The author of the best seller, as well as other contributors
          such as the illustrator (to search or sort by author name only, use author
          instead)
      - in: query
        name: isbn
        description: International Standard Book Number, 10 or 13 digitsA best seller
          may have both 10-digit and 13-digit ISBNs, and may have multiple ISBNs of
          each type
      - in: query
        name: price
        description: The publishers list price of the best seller, including decimal
          point
      - in: query
        name: publisher
        description: The standardized name of the publisher
      - in: query
        name: title
        description: The title of the best sellerWhen searching, you can specify a
          portion of a title or a full title
      responses:
        200:
          description: OK
      tags:
      - Books
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