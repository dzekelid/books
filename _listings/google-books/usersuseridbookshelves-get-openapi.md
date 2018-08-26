---
swagger: "2.0"
x-collection-name: Google Books
x-complete: 0
info:
  title: Google Books API Get Public Bookkshelves
  description: Retrieves a list of public bookshelves for the specified user.
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
  /cloudloading/addBook:
    post:
      summary: Add Book
      description: Adds a book and its contents
      operationId: books.cloudloading.addBook
      x-api-path-slug: cloudloadingaddbook-post
      parameters:
      - in: query
        name: drive_document_id
        description: A drive document id
      - in: query
        name: mime_type
        description: The document MIME type
      - in: query
        name: name
        description: The document name
      - in: query
        name: upload_client_token
      responses:
        200:
          description: OK
      tags:
      - Book
  /cloudloading/deleteBook:
    post:
      summary: Remove Book
      description: Remove the book and its contents
      operationId: books.cloudloading.deleteBook
      x-api-path-slug: cloudloadingdeletebook-post
      parameters:
      - in: query
        name: volumeId
        description: The id of the book to be removed
      responses:
        200:
          description: OK
      tags:
      - Book
  /cloudloading/updateBook:
    post:
      summary: Update Book
      description: Updates a book and its contents
      operationId: books.cloudloading.updateBook
      x-api-path-slug: cloudloadingupdatebook-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Book
  /volumes/mybooks:
    get:
      summary: Get My Books
      description: Return a list of books in My Library.
      operationId: books.volumes.mybooks.list
      x-api-path-slug: volumesmybooks-get
      parameters:
      - in: query
        name: acquireMethod
        description: How the book was acquired
      - in: query
        name: country
        description: ISO-3166-1 code to override the IP-based location
      - in: query
        name: locale
        description: ISO-639-1 language and ISO-3166-1 country code
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: processingState
        description: The processing state of the user uploaded volumes to be returned
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: startIndex
        description: Index of the first result to return (starts at 0)
      responses:
        200:
          description: OK
      tags:
      - Book
  /mylibrary/bookshelves:
    get:
      summary: Get Bookshelves
      description: Retrieves a list of bookshelves belonging to the authenticated
        user.
      operationId: books.mylibrary.bookshelves.list
      x-api-path-slug: mylibrarybookshelves-get
      parameters:
      - in: query
        name: source
        description: String to identify the originator of this request
      responses:
        200:
          description: OK
      tags:
      - Bookshelf
  /mylibrary/bookshelves/{shelf}:
    get:
      summary: Get Bookshelf
      description: Retrieves metadata for a specific bookshelf belonging to the authenticated
        user.
      operationId: books.mylibrary.bookshelves.get
      x-api-path-slug: mylibrarybookshelvesshelf-get
      parameters:
      - in: path
        name: shelf
        description: ID of bookshelf to retrieve
      - in: query
        name: source
        description: String to identify the originator of this request
      responses:
        200:
          description: OK
      tags:
      - Bookshelf
  /users/{userId}/bookshelves:
    get:
      summary: Get Public Bookkshelves
      description: Retrieves a list of public bookshelves for the specified user.
      operationId: books.bookshelves.list
      x-api-path-slug: usersuseridbookshelves-get
      parameters:
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: path
        name: userId
        description: ID of user for whom to retrieve bookshelves
      responses:
        200:
          description: OK
      tags:
      - Bookshelf
  /users/{userId}/bookshelves/{shelf}:
    get:
      summary: Get Public Bookshelf
      description: Retrieves metadata for a specific bookshelf for the specified user.
      operationId: books.bookshelves.get
      x-api-path-slug: usersuseridbookshelvesshelf-get
      parameters:
      - in: path
        name: shelf
        description: ID of bookshelf to retrieve
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: path
        name: userId
        description: ID of user for whom to retrieve bookshelves
      responses:
        200:
          description: OK
      tags:
      - Bookshelf
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