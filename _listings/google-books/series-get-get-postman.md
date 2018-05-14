{
  "info": {
    "name": "Google Books API Get Series",
    "_postman_id": "964a6618-c085-4ede-9d45-5a7613d8799b",
    "description": "Returns Series metadata for the given series ids.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "series",
      "item": [
        {
          "id": "0e3bf2a7-68e5-42d4-9889-f5f3fe498c4c",
          "name": "books.series.get",
          "request": {
            "url": "http://www.googleapis.com/books/v1/series/get?series_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns Series metadata for the given series ids"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48965697-e953-4514-b7a8-4a27db0fd8d4"
            }
          ]
        }
      ]
    }
  ]
}