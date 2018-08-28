{
  "info": {
    "name": "Eventbrite Add Series  Cancel",
    "_postman_id": "d3f4fab6-e188-48ca-a363-50675a6254f8",
    "description": "Cancels a repeating event series and all of its occurrences that are not already canceled or deleted. In order for\ncancel to be permitted, there must be no pending or completed orders for any dates in the series. Returns a boolean\nindicating success or failure of the cancel.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Series",
      "item": [
        {
          "id": "7e095d25-8719-4027-9599-2e329d09e36d",
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
              "id": "7dc059aa-0ec0-4721-8049-d351e4144c45"
            }
          ]
        },
        {
          "id": "d14aeabf-7c29-4e76-9cdb-6b78bb9a0c3b",
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
              "id": "c1c6a72f-688f-41d5-abd9-07ffd2b2c3f4"
            }
          ]
        },
        {
          "id": "5782b590-18eb-46dd-ae41-af93cd4bc42d",
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
              "id": "9b2042a4-6cbd-4cb0-b179-9813c2adae06"
            }
          ]
        },
        {
          "id": "8f143749-2eb8-4574-9931-30e9d44f252f",
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
              "id": "b3dac811-b10c-4d84-a902-408aa7f70575"
            }
          ]
        },
        {
          "id": "c9864224-e2fa-4424-ab01-8d8367be8285",
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
              "id": "d6bec27c-3aae-4516-a5c5-5ef803a3fed8"
            }
          ]
        },
        {
          "id": "f9c13171-1381-4115-8183-54652936500c",
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
              "id": "acb6c01a-6efb-489d-bc99-89c5d7f6ffeb"
            }
          ]
        }
      ]
    }
  ]
}