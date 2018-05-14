{
  "info": {
    "name": "Microsoft Graph API List Chart Series Collection",
    "_postman_id": "8efe3a44-0372-42e0-bcaa-abd3dd1eb318",
    "description": "List ChartSeriesCollection Retrieve a list of chartseries objects.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "ff799a97-4adf-427f-b263-024225d70244",
          "name": "ListChartSeriesCollection",
          "request": {
            "url": "http://graph.microsoft.com/List, , Series, Collection",
            "method": "GET",
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
            "description": "List ChartSeriesCollection Retrieve a list of chartseries objects"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "70ccfb9c-38cb-401a-86d3-81e02871269b"
            }
          ]
        }
      ]
    }
  ]
}