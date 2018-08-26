{
  "info": {
    "name": "Google Books API Get Bookshelves",
    "_postman_id": "13a4d52c-8742-4aaa-b06d-72fb7796f13a",
    "description": "Retrieves a list of bookshelves belonging to the authenticated user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "bookshelf",
      "item": [
        {
          "id": "483658bd-20e9-410e-a051-ae1736ebe94b",
          "name": "books.mylibrary.bookshelves.list",
          "request": {
            "url": "http://www.googleapis.com/books/v1/mylibrary/bookshelves?source=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a list of bookshelves belonging to the authenticated user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db80249d-de3b-49f5-aada-b9c6a4b6c86d"
            }
          ]
        }
      ]
    }
  ]
}