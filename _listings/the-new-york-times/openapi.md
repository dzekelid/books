---
swagger: "2.0"
x-collection-name: The New York Times
x-complete: 1
info:
  title: New York Times
  description: you-already-know-that-nytimes-com-is-an-unparalleled-source-of-news-and-information--but-now-its-a-premier-source-of-data-too--why-just-read-the-news-when-you-can-hack-it
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
  /books/v2/lists/{date}/{list}.json:
    get:
      summary: Best Seller List by Date
      description: You can optionally request an overview for a specific published
        date using the published_date query parameter.
      operationId: GET_lists-date-list-json
      x-api-path-slug: booksv2listsdatelist-json-get
      parameters:
      - in: query
        name: api-key
        description: The API key
        type: string
        format: string
      - in: query
        name: bestsellers-date
        description: YYYY-MM-DDThe week-ending date for the sales reflected on list-name
      - in: query
        name: isbn
        description: International Standard Book Number, 10 or 13 digits
      - in: query
        name: list-name
        description: The name of the Times best-seller list
      - in: query
        name: offset
        description: Sets the starting point of the result set
      - in: query
        name: published-date
        description: YYYY-MM-DDThe date the best-seller list was published on NYTimes
      - in: query
        name: rank
        description: The rank of the best seller on list-name as of bestsellers-date
      - in: query
        name: rank-last-week
        description: The rank of the best seller on list-name one week prior to bestsellers-date
      - in: query
        name: sort-order
        description: The default is ASC (ascending)
      - in: query
        name: weeks-on-list
        description: The number of weeks that the best seller has been on list-name,
          as of bestsellers-date
      responses:
        200:
          description: OK
      tags:
      - Books
  /books/v2/lists/overview.{format}:
    get:
      summary: Best Seller List Overview
      description: The overview service returns the top 5 books for all the Best Sellers
        lists.
      operationId: GET_lists-overview-format
      x-api-path-slug: booksv2listsoverview-format-get
      parameters:
      - in: query
        name: api-key
        description: The API key
      - in: query
        name: format
        description: The format
        type: string
        format: string
      - in: query
        name: published_date
        description: The best-seller list publication date
      responses:
        200:
          description: OK
      tags:
      - Books
  /books/v2/lists/names.{format}:
    get:
      summary: Best Seller List Names
      description: The names service returns a list of Best Sellers list names. It
        includes in the response the type of list (weekly or monthly) and when it
        was first published and last published. Lists have been added and removed
        over time. For example the Food and Diet list was added in 2013 and the Children???s
        Chapter Books list was removed in 2012. The response also includes the list_name_encoded
        which you use when calling the details service.
      operationId: GET_lists-names-format
      x-api-path-slug: booksv2listsnames-format-get
      parameters:
      - in: query
        name: api-key
        description: The API key
      - in: query
        name: format
        description: The format
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Books
---