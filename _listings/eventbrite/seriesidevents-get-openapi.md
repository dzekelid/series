---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Get Series Events
  description: Returns all of the events that belong to this repeating event series.
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
    delete:
      summary: Delete Series
      description: |-
        Deletes a repeating event series and all of its occurrences if the delete is permitted. In order for a delete to be
        permitted, there must be no pending or completed orders for any dates in the series. Returns a boolean indicating
        success or failure of the delete.
      operationId: deleteSeries
      x-api-path-slug: seriesid-delete
      responses:
        200:
          description: OK
      tags:
      - Series
  /series/{id}/publish/:
    post:
      summary: Post Series Publish
      description: |-
        Publishes a repeating event series and all of its occurrences that are not already canceled or deleted. Once a date is cancelled it can still be uncancelled and can be viewed by the public. A deleted date cannot be undeleted and cannot by viewed by the public. In order for
        publish to be permitted, the event must have all necessary information, including a name and description, an organizer,
        at least one ticket, and valid payment options. This API endpoint will return argument errors for event fields that
        fail to validate the publish requirements. Returns a boolean indicating success or failure of the publish.
      operationId: postSeriesPublish
      x-api-path-slug: seriesidpublish-post
      responses:
        200:
          description: OK
      tags:
      - Series
      - Publish
  /series/{id}/unpublish/:
    post:
      summary: Post Series Unpublish
      description: |-
        Unpublishes a repeating event series and all of its occurrences that are not already completed, canceled, or deleted. In
        order for a free series to be unpublished, it must not have any pending or completed orders for any dates, even past
        dates. In order for a paid series to be unpublished, it must not have any pending or completed orders for any dates,
        except that completed orders for past dates that have been completed and paid out do not prevent an unpublish. Returns
        a boolean indicating success or failure of the unpublish.
      operationId: postSeriesUnpublish
      x-api-path-slug: seriesidunpublish-post
      responses:
        200:
          description: OK
      tags:
      - Series
      - Unpublish
  /series/{id}/cancel/:
    post:
      summary: Post Series Cancel
      description: |-
        Cancels a repeating event series and all of its occurrences that are not already canceled or deleted. In order for
        cancel to be permitted, there must be no pending or completed orders for any dates in the series. Returns a boolean
        indicating success or failure of the cancel.
      operationId: postSeriesCancel
      x-api-path-slug: seriesidcancel-post
      responses:
        200:
          description: OK
      tags:
      - Series
      - Cancel
  /series/{id}/events/:
    get:
      summary: Get Series Events
      description: Returns all of the events that belong to this repeating event series.
      operationId: getSeriesEvents
      x-api-path-slug: seriesidevents-get
      parameters:
      - in: query
        name: order_by
        description: 'How to order the results (Valid choices are: start_asc, start_desc,
          created_asc, or created_desc)'
        type: query
      - in: query
        name: time_filter
        description: Limits results to either past or current &amp; future events
        type: query
      - in: query
        name: tracking_code
        description: Append the given tracking_code to the event URLs returned
        type: query
      responses:
        200:
          description: OK
      tags:
      - Series
      - Events
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