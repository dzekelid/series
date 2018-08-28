{
  "info": {
    "name": "Microsoft Graph API Create Chart Series",
    "_postman_id": "c7c36141-a179-4d10-ae03-a61960320a2e",
    "description": "Create ChartSeries Use this API to create a new ChartSeries.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "chart",
      "item": [
        {
          "id": "ba61ae76-d1a6-4ac4-a352-7376e9839f4e",
          "name": "CreateChartSeries",
          "request": {
            "url": "http://graph.microsoft.com/, Series",
            "method": "POST",
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
            "description": "Create ChartSeries Use this API to create a new ChartSeries"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "6737aeb3-4bf4-43e3-b9d9-c1d7081f06fe"
            }
          ]
        }
      ]
    }
  ]
}