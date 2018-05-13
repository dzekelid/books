{
  "info": {
    "name": "Google Books API Get Public Bookkshelves",
    "_postman_id": "1bc0628c-3b94-48e5-978c-73635140c2fc",
    "description": "Retrieves a list of public bookshelves for the specified user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "bookshelf",
      "item": [
        {
          "id": "97ddc93f-c8da-4e99-a7bb-d46156322a06",
          "name": "books.bookshelves.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "books",
                "v1",
                "users/:userId/bookshelves"
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
            "description": "Retrieves a list of public bookshelves for the specified user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5654518-96e0-400e-8b3b-34baf9314780"
            }
          ]
        }
      ]
    }
  ]
}