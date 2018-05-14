{
  "info": {
    "name": "Microsoft Graph API",
    "_postman_id": "e87d8c05-4a56-4522-8f81-38f46f724983",
    "description": "Microsoft Graph exposes multiple APIs from Office 365 and other Microsoft cloud services through a single endpoint: https://graph.microsoft.com. Microsoft Graph simplifies queries that would otherwise be more complex.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "chartseries",
      "item": [
        {
          "id": "82c3bb5c-6b99-40e7-afee-2b14fedf255b",
          "name": "UpdateChartseries",
          "request": {
            "url": "http://graph.microsoft.com/series",
            "method": "PATCH",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Update chartseries Update the properties of chartseries object"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "807d250e-25cd-4ab1-a31b-b0420db3e268"
            }
          ]
        }
      ]
    }
  ]
}