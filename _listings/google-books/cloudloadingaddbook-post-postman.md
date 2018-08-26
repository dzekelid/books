{
  "info": {
    "name": "Google Books API Add Book",
    "_postman_id": "d7d64bc3-4c6a-4eb8-bf36-9a61ffef9ef9",
    "description": "Adds a book and its contents",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Book",
      "item": [
        {
          "id": "00099530-750e-4fad-a9a3-ffa551d2f5ca",
          "name": "books.cloudloading.addBook",
          "request": {
            "url": "http://www.googleapis.com/books/v1/cloudloading/addBook?drive_document_id=%7B%7D&mime_type=%7B%7D&name=%7B%7D&upload_client_token=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a book and its contents"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc4c3fb2-c77b-42df-b666-c498b57ebf04"
            }
          ]
        }
      ]
    }
  ]
}