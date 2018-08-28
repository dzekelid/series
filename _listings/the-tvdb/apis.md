---
name: The TVDB
x-slug: the-tvdb
description: TheTVDB.com is a community driven database of television shows. All content
  and images on the site have been contributed by the sites users; the site uses moderated
  editing to maintain its own standards. The database schema and website are open
  source under the GNU General Public License.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
x-kinRank: "7"
x-alexaRank: "0"
tags: Series
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/the-tvdb/apis.md
specificationVersion: "0.14"
apis:
- name: The TVDB API v2 - Get Search Series
  x-api-slug: searchseries-get
  description: Allows the user to search for a series based on the following parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/the-tvdb/searchseries-get-openapi.md
- name: The TVDB API v2 - Get Search Series Params
  x-api-slug: searchseriesparams-get
  description: Returns an array of parameters to query by in the `/search/series`
    route.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/the-tvdb/searchseriesparams-get-openapi.md
- name: The TVDB API v2 - Get Series
  x-api-slug: seriesid-get
  description: Returns a series records that contains all information known about
    a particular series id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/the-tvdb/seriesid-get-openapi.md
- name: The TVDB API v2 - Head Series
  x-api-slug: seriesid-head
  description: Returns header information only about the given series ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/the-tvdb/seriesid-head-openapi.md
- name: The TVDB API v2 - Get Series Actors
  x-api-slug: seriesidactors-get
  description: Returns actors for the given series id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/the-tvdb/seriesidactors-get-openapi.md
- name: The TVDB API v2 - Get Series Episodes
  x-api-slug: seriesidepisodes-get
  description: All episodes for a given series. Paginated with 100 results per page.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/the-tvdb/seriesidepisodes-get-openapi.md
- name: The TVDB API v2 - Get Series Episodes Query
  x-api-slug: seriesidepisodesquery-get
  description: This route allows the user to query against episodes for the given
    series. The response is a paginated array of episode records that have been filtered
    down to basic information.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/the-tvdb/seriesidepisodesquery-get-openapi.md
- name: The TVDB API v2 - Get Series Episodes Query Params
  x-api-slug: seriesidepisodesqueryparams-get
  description: Returns the allowed query keys for the `/series/{id}/episodes/query`
    route
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/the-tvdb/seriesidepisodesqueryparams-get-openapi.md
- name: The TVDB API v2 - Get Series Episodes Summary
  x-api-slug: seriesidepisodessummary-get
  description: |-
    Returns a summary of the episodes and seasons available for the series.

    __Note__: Season "0" is for all episodes that are considered to be specials.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/the-tvdb/seriesidepisodessummary-get-openapi.md
- name: The TVDB API v2 - Get Series Filter
  x-api-slug: seriesidfilter-get
  description: Returns a series records, filtered by the supplied comma-separated
    list of keys. Query keys can be found at the `/series/{id}/filter/params` route.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/the-tvdb/seriesidfilter-get-openapi.md
- name: The TVDB API v2 - Get Series Filter Params
  x-api-slug: seriesidfilterparams-get
  description: Returns the list of keys available for the `/series/{id}/filter` route
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/the-tvdb/seriesidfilterparams-get-openapi.md
- name: The TVDB API v2 - Get Series Images
  x-api-slug: seriesidimages-get
  description: Returns a summary of the images for a particular series
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/the-tvdb/seriesidimages-get-openapi.md
- name: The TVDB API v2 - Get Series Images Query
  x-api-slug: seriesidimagesquery-get
  description: Query images for the given series ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/the-tvdb/seriesidimagesquery-get-openapi.md
- name: The TVDB API v2 - Get Series Images Query Params
  x-api-slug: seriesidimagesqueryparams-get
  description: Returns the allowed query keys for the `/series/{id}/images/query`
    route. Contains a parameter record for each unique `keyType`, listing values that
    will return results.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/thetvdb.jpeg
  humanURL: http://thetvdb.com
  baseURL: https://api-dev.thetvdb.com//
  tags: Televisions, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/the-tvdb/seriesidimagesqueryparams-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://the.open.movie.database.api.gallery.streamdata.io
- type: x-api-stack
  url: http://the.tvdb.stack.network
- type: x-documentation
  url: https://api.thetvdb.com/swagger
- type: x-website
  url: http://thetvdb.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---