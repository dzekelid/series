{
  "info": {
    "name": "Eventbrite Get Series  Events",
    "_postman_id": "8a25d9a0-aedd-4129-af3a-847467cf6fd2",
    "description": "Returns all of the events that belong to this repeating event series.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Series",
      "item": [
        {
          "id": "c7ee56e6-6504-4ec3-9a79-cc6aaaeca445",
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
              "id": "d5f1a383-e0cb-48ad-9efe-e429ad779c37"
            }
          ]
        },
        {
          "id": "0eab4de2-09a3-4c2a-8bed-64fc3f75ca47",
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
              "id": "e5c9f012-526f-44da-a604-4183cbb86bbe"
            }
          ]
        },
        {
          "id": "b1e5fd89-77c5-4d77-ab58-34b7bb331837",
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
              "id": "d16dc844-7f49-4199-9935-1e5a63cff6cb"
            }
          ]
        },
        {
          "id": "e881bab3-1edc-4f27-9382-91ac0e3ee34c",
          "name": "deleteSeries",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a repeating event series and all of its occurrences if the delete is permitted. In order for a delete to be\npermitted, there must be no pending or completed orders for any dates in the series. Returns a boolean indicating\nsuccess or failure of the delete."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ef74a5a-ffe8-4272-ae78-aec2308ef8a4"
            }
          ]
        },
        {
          "id": "9169c122-2de4-4aae-8714-b50ae783a6ce",
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
              "id": "712808cf-b8d9-4356-b393-8dd9e6f50318"
            }
          ]
        },
        {
          "id": "643c35dc-3dad-41a9-abed-395e82392fa9",
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
              "id": "a65bd13f-c3b9-444f-8b45-96ed51ab34ec"
            }
          ]
        },
        {
          "id": "f092f7f5-54f8-480f-a271-280418c16477",
          "name": "postSeriesCancel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "series/:id/cancel/"
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
            "description": "Cancels a repeating event series and all of its occurrences that are not already canceled or deleted. In order for\ncancel to be permitted, there must be no pending or completed orders for any dates in the series. Returns a boolean\nindicating success or failure of the cancel."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a4b6ee8-91f4-422c-b7d2-509ebac23b17"
            }
          ]
        },
        {
          "id": "02e26477-db92-4a9e-b99e-d75ed7b3359b",
          "name": "getSeriesEvents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "series/:id/events/"
              ],
              "query": [
                {
                  "key": "order_by",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "time_filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
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
            "description": "Returns all of the events that belong to this repeating event series."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "904e99d2-a49d-4d4a-ac12-66bcb3d455f8"
            }
          ]
        }
      ]
    }
  ]
}