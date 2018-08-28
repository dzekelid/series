---
swagger: "2.0"
x-collection-name: The TVDB
x-complete: 0
info:
  title: The TVDB Get Series Images Query Params
  description: Returns the allowed query keys for the `/series/{id}/images/query`
    route. Contains a parameter record for each unique `keyType`, listing values that
    will return results.
  version: 2.1.2
host: api-dev.thetvdb.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search/series:
    get:
      summary: Get Search Series
      description: Allows the user to search for a series based on the following parameters.
      operationId: search.series.get
      x-api-path-slug: searchseries-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Search
      - Series
  /search/series/params:
    get:
      summary: Get Search Series Params
      description: Returns an array of parameters to query by in the `/search/series`
        route.
      operationId: search.series.params.get
      x-api-path-slug: searchseriesparams-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - Search
      - Series
      - Params
  /series/{id}:
    get:
      summary: Get Series
      description: Returns a series records that contains all information known about
        a particular series id.
      operationId: series.id.get
      x-api-path-slug: seriesid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
    head:
      summary: Head Series
      description: Returns header information only about the given series ID.
      operationId: series.id.head
      x-api-path-slug: seriesid-head
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
  /series/{id}/actors:
    get:
      summary: Get Series Actors
      description: Returns actors for the given series id
      operationId: series.id.actors.get
      x-api-path-slug: seriesidactors-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
      - Actors
  /series/{id}/episodes:
    get:
      summary: Get Series Episodes
      description: All episodes for a given series. Paginated with 100 results per
        page.
      operationId: series.id.episodes.get
      x-api-path-slug: seriesidepisodes-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
      - Episodes
  /series/{id}/episodes/query:
    get:
      summary: Get Series Episodes Query
      description: This route allows the user to query against episodes for the given
        series. The response is a paginated array of episode records that have been
        filtered down to basic information.
      operationId: series.id.episodes.query.get
      x-api-path-slug: seriesidepisodesquery-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
      - Episodes
      - Query
  /series/{id}/episodes/query/params:
    get:
      summary: Get Series Episodes Query Params
      description: Returns the allowed query keys for the `/series/{id}/episodes/query`
        route
      operationId: series.id.episodes.query.params.get
      x-api-path-slug: seriesidepisodesqueryparams-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
      - Episodes
      - Query
      - Params
  /series/{id}/episodes/summary:
    get:
      summary: Get Series Episodes Summary
      description: |-
        Returns a summary of the episodes and seasons available for the series.

        __Note__: Season "0" is for all episodes that are considered to be specials.
      operationId: series.id.episodes.summary.get
      x-api-path-slug: seriesidepisodessummary-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
      - Episodes
      - Summary
  /series/{id}/filter:
    get:
      summary: Get Series Filter
      description: Returns a series records, filtered by the supplied comma-separated
        list of keys. Query keys can be found at the `/series/{id}/filter/params`
        route.
      operationId: series.id.filter.get
      x-api-path-slug: seriesidfilter-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
      - Filter
  /series/{id}/filter/params:
    get:
      summary: Get Series Filter Params
      description: Returns the list of keys available for the `/series/{id}/filter`
        route
      operationId: series.id.filter.params.get
      x-api-path-slug: seriesidfilterparams-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
      - Filter
      - Params
  /series/{id}/images:
    get:
      summary: Get Series Images
      description: Returns a summary of the images for a particular series
      operationId: series.id.images.get
      x-api-path-slug: seriesidimages-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
      - Images
  /series/{id}/images/query:
    get:
      summary: Get Series Images Query
      description: Query images for the given series ID.
      operationId: series.id.images.query.get
      x-api-path-slug: seriesidimagesquery-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
      - Images
      - Query
  /series/{id}/images/query/params:
    get:
      summary: Get Series Images Query Params
      description: Returns the allowed query keys for the `/series/{id}/images/query`
        route. Contains a parameter record for each unique `keyType`, listing values
        that will return results.
      operationId: series.id.images.query.params.get
      x-api-path-slug: seriesidimagesqueryparams-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
      - Images
      - Query
      - Params
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