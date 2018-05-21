{
  "info": {
    "name": "Eventbrite Add Series  Publish",
    "_postman_id": "8418c5e6-fb31-4c1e-a81e-48f1def785d8",
    "description": "Publishes a repeating event series and all of its occurrences that are not already canceled or deleted. Once a date is cancelled it can still be uncancelled and can be viewed by the public. A deleted date cannot be undeleted and cannot by viewed by the public. In order for\npublish to be permitted, the event must have all necessary information, including a name and description, an organizer,\nat least one ticket, and valid payment options. This API endpoint will return argument errors for event fields that\nfail to validate the publish requirements. Returns a boolean indicating success or failure of the publish.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Series",
      "item": [
        {
          "id": "57a11a01-5619-47bc-bf83-2311402ebe36",
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
              "id": "94baba86-bc85-4452-a5c2-241b50857ca7"
            }
          ]
        },
        {
          "id": "3ede53cd-a5e3-41b8-9670-52bfbb133f10",
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
              "id": "649121e5-696a-402e-b64e-17d941023a83"
            }
          ]
        },
        {
          "id": "06bdc9bf-71f3-4979-822c-3e22f7f7309e",
          "name": "postSeries1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "series/:id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a repeating event series parent object, and optionally also creates more event dates or updates or deletes\nexisting event dates in the series. In order for a series date to be deleted or updated, there must be no pending or\ncompleted orders for that date."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6375ea16-c90a-40c8-ab22-3baa19b7b591"
            }
          ]
        },
        {
          "id": "3ca7688e-4dfc-4c1a-a073-d6c52022d4cf",
          "name": "postSeriesPublish",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "series/:id/publish/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Publishes a repeating event series and all of its occurrences that are not already canceled or deleted. Once a date is cancelled it can still be uncancelled and can be viewed by the public. A deleted date cannot be undeleted and cannot by viewed by the public. In order for\npublish to be permitted, the event must have all necessary information, including a name and description, an organizer,\nat least one ticket, and valid payment options. This API endpoint will return argument errors for event fields that\nfail to validate the publish requirements. Returns a boolean indicating success or failure of the publish."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6093f3c3-467d-464d-bb2b-83f6759ac3ad"
            }
          ]
        }
      ]
    }
  ]
}