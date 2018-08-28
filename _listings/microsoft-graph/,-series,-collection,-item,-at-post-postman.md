{
  "info": {
    "name": "Microsoft Graph API Chart Series Collection Item At",
    "_postman_id": "e88fcf91-30ea-43e5-885c-cfb65fadb7aa",
    "description": "ChartSeriesCollection: ItemAt Retrieves a series based on its position in the collection",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "chart",
      "item": [
        {
          "id": "1be88ea4-249c-47de-9b1c-4a9920ab64aa",
          "name": "ChartSeriesCollection:ItemAt",
          "request": {
            "url": "http://graph.microsoft.com/, Series, Collection, Item, At",
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
            "description": "ChartSeriesCollection: ItemAt Retrieves a series based on its position in the collection"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "eef522ca-bcb5-4d27-a196-ba56168e6ec7"
            }
          ]
        }
      ]
    }
  ]
}