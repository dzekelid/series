{
  "info": {
    "name": "Eventbrite Delete Series",
    "_postman_id": "93465567-7108-4573-a9a1-cbec7f35caeb",
    "description": "Deletes a repeating event series and all of its occurrences if the delete is permitted. In order for a delete to be\npermitted, there must be no pending or completed orders for any dates in the series. Returns a boolean indicating\nsuccess or failure of the delete.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Series",
      "item": [
        {
          "id": "243388f1-9c1e-4262-b924-2afd359cc05f",
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
              "id": "efc66e9b-70aa-4ca6-aa8d-454a7c2b37f0"
            }
          ]
        },
        {
          "id": "8904e19c-ba25-4ad7-8026-08646a9bfea9",
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
              "id": "3b42cc48-71ac-4e60-8068-d4ae2d46a37b"
            }
          ]
        },
        {
          "id": "86d507a2-313e-4262-be7b-2fb7ba2dedbc",
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
              "id": "ec595289-bdd9-4ec4-80d5-249e86fc905f"
            }
          ]
        },
        {
          "id": "55654a1e-3d27-4c1c-a732-cabcc15adc70",
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
              "id": "7719918f-55fc-4560-a4f4-5f024979424b"
            }
          ]
        },
        {
          "id": "b5cebe92-9333-4b9c-91ad-2fbf6941e39c",
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
              "id": "1890213f-e53a-4e6c-9954-18ab3a9b875b"
            }
          ]
        },
        {
          "id": "f9cbd81f-15f1-44f5-a967-0757a520f720",
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
              "id": "72fb8b77-f82b-4855-8623-0f497553e775"
            }
          ]
        },
        {
          "id": "f8e82f05-5e46-41a5-8916-cda483377d34",
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
              "id": "32a054cc-8772-4496-9f54-9188438508e3"
            }
          ]
        }
      ]
    }
  ]
}