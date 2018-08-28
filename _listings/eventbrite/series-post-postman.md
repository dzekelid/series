{
  "info": {
    "name": "Eventbrite Add Series",
    "_postman_id": "2b439712-faf4-44d0-a719-28f49d4d550e",
    "description": "Creates a new repeating event series. The POST data must include information for at least one event date in the series.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Series",
      "item": [
        {
          "id": "c49b229f-4e68-46bb-a69a-06eb0e808c65",
          "name": "postSeries",
          "request": {
            "url": "http://www.eventbriteapi.com/v3/series/",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new repeating event series. The POST data must include information for at least one event date in the series."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2fb8726d-48c4-49c7-9401-9b40197582db"
            }
          ]
        }
      ]
    }
  ]
}