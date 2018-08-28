---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Post Series
  description: |-
    Updates a repeating event series parent object, and optionally also creates more event dates or updates or deletes
    existing event dates in the series. In order for a series date to be deleted or updated, there must be no pending or
    completed orders for that date.
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /series/:
    post:
      summary: Post Series
      description: Creates a new repeating event series. The POST data must include
        information for at least one event date in the series.
      operationId: postSeries
      x-api-path-slug: series-post
      responses:
        200:
          description: OK
      tags:
      - Series
  /series/{id}/:
    get:
      summary: Get Series
      description: Returns a repeating event series parent object for the specified
        repeating event series.
      operationId: getSeries
      x-api-path-slug: seriesid-get
      parameters:
      - in: query
        name: tracking_code
        description: Append the given tracking_code to the event URLs returned
        type: query
      responses:
        200:
          description: OK
      tags:
      - Series
    post:
      summary: Post Series
      description: |-
        Updates a repeating event series parent object, and optionally also creates more event dates or updates or deletes
        existing event dates in the series. In order for a series date to be deleted or updated, there must be no pending or
        completed orders for that date.
      operationId: postSeries
      x-api-path-slug: seriesid-post
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