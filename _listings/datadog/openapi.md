swagger: "2.0"
x-collection-name: Datadog
x-complete: 1
info:
  title: DataDog Merged API
  version: 1.0.0
basePath: api/v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /series:
    post:
      summary: Add Series
      description: |-
        The metrics end-point allows you to post time-series data that can be
                  graphed on Datadog's dashboards.
      operationId: postSeries
      x-api-path-slug: series-post
      parameters:
      - in: query
        name: '[[POSIX_timestamp, numeric_value], ...]'
        description: Note that the timestamp should be in seconds, must be current,
          and the numeric value is a 32bit float gauge-type value
        type: string
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Series