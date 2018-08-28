swagger: "2.0"
x-collection-name: The TVDB
x-complete: 1
info:
  title: The TVDB API v2
  description: api-v2-targets-v1-functionality-with-a-few-minor-additions--the-api-is-accessible-via-httpsapi-thetvdb-com-and-provides-the-following-rest-endpoints-in-json-format-how-to-use-this-api-documentationyou-may-browse-the-api-routes-without-authentication-but-if-you-wish-to-send-requests-to-the-api-and-see-response-data-then-you-must-authenticate-1--obtain-a-jwt-token-by-posting--to-the-login-route-in-the-authentication-section-with-your-api-key-and-credentials-1--paste-the-jwt-token-from-the-response-into-the-jwt-token-field-at-the-top-of-the-page-and-click-the-add-token-button-you-will-now-be-able-to-use-the-remaining-routes-to-send-requests-to-the-api-and-get-a-response-language-selectionlanguage-selection-is-done-via-the-acceptlanguage-header--at-the-moment-you-may-only-pass-one-language-abbreviation-in-the-header-at-a-time--valid-language-abbreviations-can-be-found-at-the-languages-route--authenticationauthentication-to-use-the-api-is-similar-to-the-howto-section-above--users-must-post-to-the-login-route-with-their-api-key-and-credentials-in-the-following-format-in-order-to-obtain-a-jwt-token-apikeyapikeyusernameusernameuserkeyuserkeynote-that-the-username-and-key-are-only-required-for-the-user-routes--the-users-key-is-labled-account-identifier-in-the-account-section-of-the-main-site-the-token-is-then-used-in-all-subsequent-requests-by-providing-it-in-the-authorization-header--the-header-will-look-like-authorization-bearer-yourjwttoken--currently-the-token-expires-after-24-hours--you-can-get-the-refresh-token-route-to-extend-that-expiration-date-versioningyou-may-request-a-different-version-of-the-api-by-including-an-accept-header-in-your-request-with-the-following-format-acceptapplicationvnd-thetvdb-vversion--this-documentation-automatically-uses-the-version-seen-at-the-top-and-bottom-of-the-page-
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