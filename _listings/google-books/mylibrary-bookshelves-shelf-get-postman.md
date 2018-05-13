{
  "info": {
    "name": "Google Books API Get Bookshelf",
    "_postman_id": "2023abbf-24d3-4ba8-9d28-b83945721d71",
    "description": "Retrieves metadata for a specific bookshelf belonging to the authenticated user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "bookshelf",
      "item": [
        {
          "id": "61baae40-f1ee-47f9-97c4-9bd3131767a9",
          "name": "books.mylibrary.bookshelves.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "books",
                "v1",
                "mylibrary/bookshelves/:shelf"
              ],
              "query": [
                {
                  "key": "source",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "shelf",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves metadata for a specific bookshelf belonging to the authenticated user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc5382fd-1376-4ab7-b864-5a45bbff56f6"
            }
          ]
        }
      ]
    }
  ]
}