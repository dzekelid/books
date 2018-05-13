{
  "info": {
    "name": "Google Books API Get Public Bookshelf",
    "_postman_id": "73f70ec4-fe15-438e-b757-0be3b4751a12",
    "description": "Retrieves metadata for a specific bookshelf for the specified user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "bookshelf",
      "item": [
        {
          "id": "03867344-f4cb-4365-b9a9-f27fda9c48a2",
          "name": "books.bookshelves.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "books",
                "v1",
                "users/:userId/bookshelves/:shelf"
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
                },
                {
                  "id": "userId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves metadata for a specific bookshelf for the specified user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd8e8f74-742e-49fa-bdc1-0ff0ac98a15c"
            }
          ]
        }
      ]
    }
  ]
}