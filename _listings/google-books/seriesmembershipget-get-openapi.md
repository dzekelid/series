---
swagger: "2.0"
x-collection-name: Google Books
x-complete: 0
info:
  title: Google Books API Get Series Membership
  description: Returns Series membership data given the series id.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /books/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /series/get:
    get:
      summary: Get Series
      description: Returns Series metadata for the given series ids.
      operationId: books.series.get
      x-api-path-slug: seriesget-get
      parameters:
      - in: query
        name: series_id
        description: String that identifies the series
      responses:
        200:
          description: OK
      tags:
      - Series
  /series/membership/get:
    get:
      summary: Get Series Membership
      description: Returns Series membership data given the series id.
      operationId: books.series.membership.get
      x-api-path-slug: seriesmembershipget-get
      parameters:
      - in: query
        name: page_size
        description: Number of maximum results per page to be included in the response
      - in: query
        name: page_token
        description: The value of the nextToken from the previous page
      - in: query
        name: series_id
        description: String that identifies the series
      responses:
        200:
          description: OK
      tags:
      - Series
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