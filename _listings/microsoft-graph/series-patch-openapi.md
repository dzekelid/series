---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph API Update Chartseries
  description: Update chartseries Update the properties of chartseries object.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  List, , Series, Collection:
    get:
      summary: List Chart Series Collection
      description: List ChartSeriesCollection Retrieve a list of chartseries objects.
      operationId: ListChartSeriesCollection
      x-api-path-slug: list--series-collection-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      responses:
        200:
          description: OK
      tags:
      - List
      - Chart
      - Series
      - Collection
  ', Series':
    post:
      summary: Create Chart Series
      description: Create ChartSeries Use this API to create a new ChartSeries.
      operationId: CreateChartSeries
      x-api-path-slug: series-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      responses:
        200:
          description: OK
      tags:
      - Chart
      - Series
    get:
      summary: Get Chart Series
      description: Get ChartSeries Retrieve the properties and relationships of chartseries
        object.
      operationId: GetChartSeries
      x-api-path-slug: series-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      responses:
        200:
          description: OK
      tags:
      - Chart
      - Series
  series:
    patch:
      summary: Update Chartseries
      description: Update chartseries Update the properties of chartseries object.
      operationId: UpdateChartseries
      x-api-path-slug: series-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      responses:
        200:
          description: OK
      tags:
      - Chartseries
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---