{
  "info": {
    "name": "Google Books API Get Series Membership",
    "_postman_id": "3933c7f5-afd4-4c0f-9254-6f9e473a119b",
    "description": "Returns Series membership data given the series id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "series",
      "item": [
        {
          "id": "492ad52a-bac1-4acd-aab4-9403b8887b21",
          "name": "books.series.membership.get",
          "request": {
            "url": "http://www.googleapis.com/books/v1/series/membership/get?page_size=%7B%7D&page_token=%7B%7D&series_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns Series membership data given the series id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1134c9d-0a25-44d6-956f-fba2aab7808c"
            }
          ]
        }
      ]
    }
  ]
}