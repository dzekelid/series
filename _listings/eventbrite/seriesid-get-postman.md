{
  "info": {
    "name": "Eventbrite Get Series",
    "_postman_id": "ac870c11-8517-45fd-8e67-f19e6d5bb297",
    "description": "Returns a repeating event series parent object for the specified repeating event series.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Series",
      "item": [
        {
          "id": "485d296f-ba13-4f35-8621-e4d4948c1bb2",
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
              "id": "d1571c1c-6b08-4286-9aa9-409fbcc41c0f"
            }
          ]
        },
        {
          "id": "04e96934-9250-41c5-b820-a56a8a49fea4",
          "name": "getSeries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "series/:id/"
              ],
              "query": [
                {
                  "key": "tracking_code",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a repeating event series parent object for the specified repeating event series."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca6210a0-bc51-482e-a475-3182196bbbe6"
            }
          ]
        }
      ]
    }
  ]
}