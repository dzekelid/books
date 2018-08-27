{
  "info": {
    "name": "Google Books API Remove Book",
    "_postman_id": "462c4844-2936-4289-a934-c969995f82ac",
    "description": "Remove the book and its contents",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Book",
      "item": [
        {
          "id": "54bacf37-fb54-4637-b727-19da644d0b4a",
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
              "id": "4547942b-2a36-4831-a758-df8920aaefc9"
            }
          ]
        },
        {
          "id": "28ca1d6a-751c-4dd2-9c4b-f590edf4843c",
          "name": "books.cloudloading.deleteBook",
          "request": {
            "url": "http://www.googleapis.com/books/v1/cloudloading/deleteBook?volumeId=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Remove the book and its contents"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df3e8410-79eb-4ad0-824c-f2e0ab0c9851"
            }
          ]
        }
      ]
    }
  ]
}