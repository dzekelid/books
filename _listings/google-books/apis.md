---
name: Google Books
x-slug: google-books
description: Google Books is our effort to make book content more discoverable on
  the Web. Using the Google Books API, your application can perform full-text searches
  and retrieve book information, viewability and eBook availability. You can also
  manage your personal bookshelves.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
  Shot 2017-03-16 at 4.28.26 PM.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Books
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/apis.md
specificationVersion: "0.14"
apis:
- name: Books - Add Book
  x-api-slug: cloudloadingaddbook-post
  description: Adds a book and its contents
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/cloudloadingaddbook-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/cloudloadingaddbook-post-openapi.md
- name: Books - Remove Book
  x-api-slug: cloudloadingdeletebook-post
  description: Remove the book and its contents
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/cloudloadingdeletebook-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/cloudloadingdeletebook-post-openapi.md
- name: Books - Update Book
  x-api-slug: cloudloadingupdatebook-post
  description: Updates a book and its contents
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/cloudloadingupdatebook-post-openapi.md
- name: Books - Get My Books
  x-api-slug: volumesmybooks-get
  description: Return a list of books in My Library.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/volumesmybooks-get-openapi.md
- name: Books - Get Bookshelves
  x-api-slug: mylibrarybookshelves-get
  description: Retrieves a list of bookshelves belonging to the authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/mylibrarybookshelves-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/mylibrarybookshelves-get-openapi.md
- name: Books - Get Bookshelf
  x-api-slug: mylibrarybookshelvesshelf-get
  description: Retrieves metadata for a specific bookshelf belonging to the authenticated
    user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/mylibrarybookshelvesshelf-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/mylibrarybookshelvesshelf-get-openapi.md
- name: Books - Get Public Bookkshelves
  x-api-slug: usersuseridbookshelves-get
  description: Retrieves a list of public bookshelves for the specified user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/usersuseridbookshelves-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/usersuseridbookshelves-get-openapi.md
- name: Books - Get Public Bookshelf
  x-api-slug: usersuseridbookshelvesshelf-get
  description: Retrieves metadata for a specific bookshelf for the specified user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/usersuseridbookshelvesshelf-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/usersuseridbookshelvesshelf-get-openapi.md
- name: Books - Add Book
  x-api-slug: cloudloadingaddbook-post
  description: Adds a book and its contents
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/cloudloadingaddbook-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/cloudloadingaddbook-post-openapi.md
- name: Books - Remove Book
  x-api-slug: cloudloadingdeletebook-post
  description: Remove the book and its contents
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/cloudloadingdeletebook-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/cloudloadingdeletebook-post-openapi.md
- name: Books - Update Book
  x-api-slug: cloudloadingupdatebook-post
  description: Updates a book and its contents
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/cloudloadingupdatebook-post-openapi.md
- name: Books - Get My Books
  x-api-slug: volumesmybooks-get
  description: Return a list of books in My Library.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/volumesmybooks-get-openapi.md
- name: Books - Get Bookshelves
  x-api-slug: mylibrarybookshelves-get
  description: Retrieves a list of bookshelves belonging to the authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/mylibrarybookshelves-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/mylibrarybookshelves-get-openapi.md
- name: Books - Get Bookshelf
  x-api-slug: mylibrarybookshelvesshelf-get
  description: Retrieves metadata for a specific bookshelf belonging to the authenticated
    user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/mylibrarybookshelvesshelf-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/mylibrarybookshelvesshelf-get-openapi.md
- name: Books - Get Public Bookkshelves
  x-api-slug: usersuseridbookshelves-get
  description: Retrieves a list of public bookshelves for the specified user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/usersuseridbookshelves-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/usersuseridbookshelves-get-openapi.md
- name: Books - Get Public Bookshelf
  x-api-slug: usersuseridbookshelvesshelf-get
  description: Retrieves metadata for a specific bookshelf for the specified user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/usersuseridbookshelvesshelf-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/usersuseridbookshelvesshelf-get-openapi.md
- name: Books - Add Book
  x-api-slug: cloudloadingaddbook-post
  description: Adds a book and its contents
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/cloudloadingaddbook-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/cloudloadingaddbook-post-openapi.md
- name: Books - Remove Book
  x-api-slug: cloudloadingdeletebook-post
  description: Remove the book and its contents
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/cloudloadingdeletebook-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/cloudloadingdeletebook-post-openapi.md
- name: Books - Update Book
  x-api-slug: cloudloadingupdatebook-post
  description: Updates a book and its contents
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/cloudloadingupdatebook-post-openapi.md
- name: Books - Get My Books
  x-api-slug: volumesmybooks-get
  description: Return a list of books in My Library.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/volumesmybooks-get-openapi.md
- name: Books - Get Bookshelves
  x-api-slug: mylibrarybookshelves-get
  description: Retrieves a list of bookshelves belonging to the authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/mylibrarybookshelves-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/mylibrarybookshelves-get-openapi.md
- name: Books - Get Bookshelf
  x-api-slug: mylibrarybookshelvesshelf-get
  description: Retrieves metadata for a specific bookshelf belonging to the authenticated
    user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/mylibrarybookshelvesshelf-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/mylibrarybookshelvesshelf-get-openapi.md
- name: Books - Get Public Bookkshelves
  x-api-slug: usersuseridbookshelves-get
  description: Retrieves a list of public bookshelves for the specified user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/usersuseridbookshelves-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/usersuseridbookshelves-get-openapi.md
- name: Books - Get Public Bookshelf
  x-api-slug: usersuseridbookshelvesshelf-get
  description: Retrieves metadata for a specific bookshelf for the specified user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/usersuseridbookshelvesshelf-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/books/master/_listings/google-books/usersuseridbookshelvesshelf-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.biquery.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.books.stack.network
- type: x-blog
  url: http://booksearch.blogspot.com
- type: x-blog-rss
  url: http://booksearch.blogspot.com/feeds/posts/default?alt=rss
- type: x-branding-guidelines
  url: https://developers.google.com/books/branding
- type: x-code
  url: https://developers.google.com/books/docs/v1/libraries
- type: x-documentation
  url: https://developers.google.com/books/docs/overview
- type: x-embeddable
  url: https://developers.google.com/books/docs/viewer/developers_guide
- type: x-partners
  url: https://books.google.com/intl/en/googlebooks/partners/
- type: x-privacy-policy
  url: https://books.google.com/intl/en/policies/privacy/
- type: x-terms-of-service
  url: https://developers.google.com/books/terms.html
- type: x-website
  url: https://developers.google.com/books/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---