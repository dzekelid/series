{
  "info": {
    "name": "Eventbrite Add Series  Events",
    "_postman_id": "2a7e87d8-6b8e-4d49-bc4d-5e14aef1982f",
    "description": "Creates more event dates or updates or deletes existing event dates in a repeating event series. In order for a series\ndate to be deleted or updated, there must be no pending or completed orders for that date.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Series",
      "item": [
        {
          "id": "8f67f2b0-c437-4e6e-9028-14470f71ce24",
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
              "id": "fe4157ae-c58d-4c0f-9ebb-5ab3fcbfd135"
            }
          ]
        },
        {
          "id": "3df9cc2c-53db-4219-8498-7529742915f1",
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
              "id": "b524ec28-cdb4-4ee7-949b-07203901ad03"
            }
          ]
        },
        {
          "id": "5b9b1f52-7a8d-4c4c-85ce-2615b9c45f97",
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
              "id": "67c28a36-4fad-4820-9b15-7e06de0e02c0"
            }
          ]
        },
        {
          "id": "9e59623e-e7fe-4ebc-a13b-0be0c7c38432",
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
              "id": "e924ae6d-8d99-4105-9bc8-916df14c827e"
            }
          ]
        },
        {
          "id": "a1964b23-75f5-4ffd-97eb-d004460f61b5",
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
              "id": "6606d4f2-8234-42c6-a3e3-8bc3e58420d7"
            }
          ]
        },
        {
          "id": "e1d5ae6a-c7ab-4e67-9f3c-d2a397b96345",
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
              "id": "4faf36b3-6d79-466b-be8b-86f979d468aa"
            }
          ]
        },
        {
          "id": "52a1eb3b-9c49-4df1-b400-0326c9b2f2e9",
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
              "id": "c8a49e1d-67b2-4710-a5d1-0b0d0e215c88"
            }
          ]
        },
        {
          "id": "0d0656ad-4dee-45e0-91ac-0bd3b44d0728",
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
              "id": "432e0f0f-3781-41b8-8f78-9b227b9011db"
            }
          ]
        },
        {
          "id": "30799ce3-a05b-45d2-a80f-842e4734c31b",
          "name": "postSeriesEvents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbriteapi.com",
              "path": [
                "v3",
                "series/:id/events/"
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
            "description": "Creates more event dates or updates or deletes existing event dates in a repeating event series. In order for a series\ndate to be deleted or updated, there must be no pending or completed orders for that date."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fcae5ffa-8956-47d2-88f7-da248e7e9bd9"
            }
          ]
        }
      ]
    }
  ]
}