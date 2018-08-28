{
  "info": {
    "name": "Microsoft Graph API Get Chart Series",
    "_postman_id": "74b332c6-8b5a-413b-8b84-0129df954fad",
    "description": "Get ChartSeries Retrieve the properties and relationships of chartseries object.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "chart",
      "item": [
        {
          "id": "22f42c3c-bcf4-434d-a941-44c7e7498aaf",
          "name": "GetChartSeries",
          "request": {
            "url": "http://graph.microsoft.com/, Series",
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
            "description": "Get ChartSeries Retrieve the properties and relationships of chartseries object"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "0dfe25d9-820b-4490-ba5b-95669a1e9f0b"
            }
          ]
        }
      ]
    }
  ]
}