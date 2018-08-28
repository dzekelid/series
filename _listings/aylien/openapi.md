swagger: "2.0"
x-collection-name: Aylien
x-complete: 1
info:
  title: AYLIEN News API
  description: the-aylien-news-api-is-the-most-powerful-way-of-sourcing-searching-and-syndicating-analyzed-and-enriched-news-content--it-is-accessed-by-sending-http-requests-to-our-server-which-returns-information-to-your-client-
  termsOfService: https://newsapi.aylien.com/tos
  contact:
    name: API support
    url: https://newsapi.aylien.com/
    email: support@aylien.com
  version: 1.0.0
host: api.newsapi.aylien.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /time_series:
    get:
      summary: List time series
      description: The time series endpoint allows you to track information contained
        in stories over time. This information can be anything from mentions of a
        topic or entities, sentiment about a topic, or the volume of stories published
        by a source, to name but a few. The full list of parameters is given below.
        Using the [Date Math Syntax](https://newsapi.aylien.com/docs/working-with-dates),
        you can easily set your query to return information from any time period,
        from the current point in time to when the News API started collecting stories.
        The returned information can be rounded to a time also specified by you, for
        example by setting the results into hourly, daily, or weekly data points.
      operationId: listTimeSeries
      x-api-path-slug: time-series-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - News
      - List
      - Time
      - Series