---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraphmicrosoftcom-microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex
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
  ', Series, Collection, Item, At':
    post:
      summary: Chart Series Collection Item At
      description: 'ChartSeriesCollection: ItemAt Retrieves a series based on its
        position in the collection'
      operationId: ChartSeriesCollection:ItemAt
      x-api-path-slug: series-collection-item-at-post
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
      - Collection
      - Item
      - At
---