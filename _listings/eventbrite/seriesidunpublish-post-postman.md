{
  "info": {
    "name": "Eventbrite Add Series  Unpublish",
    "_postman_id": "fd39400a-4261-40f4-b716-18637d76abd0",
    "description": "Unpublishes a repeating event series and all of its occurrences that are not already completed, canceled, or deleted. In\norder for a free series to be unpublished, it must not have any pending or completed orders for any dates, even past\ndates. In order for a paid series to be unpublished, it must not have any pending or completed orders for any dates,\nexcept that completed orders for past dates that have been completed and paid out do not prevent an unpublish. Returns\na boolean indicating success or failure of the unpublish.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Series",
      "item": [
        {
          "id": "ed28fca4-f933-4a51-b289-fbe5c03883f2",
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
              "id": "a0206558-0735-4c8a-b4c2-4bbc001df558"
            }
          ]
        },
        {
          "id": "621e7505-ae27-4690-b710-91cf9f489b1b",
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
              "id": "08255a4f-db66-471d-87f6-96601cb43037"
            }
          ]
        },
        {
          "id": "0098f784-e114-4a38-94ef-cddede706737",
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
              "id": "5a4de085-5e94-469f-88b8-2082a39d15fa"
            }
          ]
        },
        {
          "id": "ae4f447f-a045-4b67-9302-452c13d05f27",
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
              "id": "e7a2b04c-f6b9-4816-a270-d7a0c846f846"
            }
          ]
        },
        {
          "id": "ee8d5a64-2667-4602-a1c2-0ad05e89bff1",
          "name": "postSeriesUnpublish",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "series/:id/unpublish/"
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
            "description": "Unpublishes a repeating event series and all of its occurrences that are not already completed, canceled, or deleted. In\norder for a free series to be unpublished, it must not have any pending or completed orders for any dates, even past\ndates. In order for a paid series to be unpublished, it must not have any pending or completed orders for any dates,\nexcept that completed orders for past dates that have been completed and paid out do not prevent an unpublish. Returns\na boolean indicating success or failure of the unpublish."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61f8e1a1-b622-418f-92d9-0dc7e9346f77"
            }
          ]
        }
      ]
    }
  ]
}