---
name: Firebase
x-slug: firebase
description: Firebase is a mobile platform that helps you quicklydevelophigh-quality
  apps,growyour user base, andearnmore money. Firebase is made up of complementary
  features that you can mix-and-match to fit your needs.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
x-kinRank: "9"
x-alexaRank: ""
tags: Series
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/firebase/apis.md
specificationVersion: "0.14"
apis:
- name: Firebase Get Sample Series
  x-api-slug: firebase
  description: |-
    Lists PerfSampleSeries for a given Step.

    The request provides an optional filter which specifies one or more PerfMetricsType to include in the result; if none returns all. The resulting PerfSampleSeries are sorted by ids.

    May return any of the following canonical error codes: - NOT_FOUND - The containing Step does not exist
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://firebase.google.com/
  baseURL: https://{project_id].firebaseio.co}////{projectId}/histories/{historyId}/executions/{executionId}/steps/{stepId}/perfSampleSeries
  tags: Sample Series
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/firebase/projectidhistorieshistoryidexecutionsexecutionidstepsstepidperfsampleseries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/firebase/projectidhistorieshistoryidexecutionsexecutionidstepsstepidperfsampleseries-get-openapi.md
- name: Firebase Create Sample Series
  x-api-slug: firebase
  description: |-
    Creates a PerfSampleSeries.

    May return any of the following error code(s): - ALREADY_EXISTS - PerfMetricSummary already exists for the given Step - NOT_FOUND - The containing Step does not exist
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://firebase.google.com/
  baseURL: https://{project_id].firebaseio.co}////{projectId}/histories/{historyId}/executions/{executionId}/steps/{stepId}/perfSampleSeries
  tags: Sample Series
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/firebase/projectidhistorieshistoryidexecutionsexecutionidstepsstepidperfsampleseries-post-openapi.md
- name: Firebase Get Sample Series
  x-api-slug: firebase
  description: |-
    Gets a PerfSampleSeries.

    May return any of the following error code(s): - NOT_FOUND - The specified PerfSampleSeries does not exist
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://firebase.google.com/
  baseURL: https://{project_id].firebaseio.co}////{projectId}/histories/{historyId}/executions/{executionId}/steps/{stepId}/perfSampleSeries/{sampleSeriesId}
  tags: Sample Series
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/firebase/projectidhistorieshistoryidexecutionsexecutionidstepsstepidperfsampleseriessampleseriesid-get-openapi.md
- name: Firebase Get Sample Series
  x-api-slug: firebase
  description: |-
    Lists the Performance Samples of a given Sample Series - The list results are sorted by timestamps ascending - The default page size is 500 samples; and maximum size allowed 5000 - The response token indicates the last returned PerfSample timestamp - When the results size exceeds the page size, submit a subsequent request including the page token to return the rest of the samples up to the page limit

    May return any of the following canonical error codes: - OUT_OF_RANGE - The specified request page_token is out of valid range - NOT_FOUND - The containing PerfSampleSeries does not exist
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://firebase.google.com/
  baseURL: https://{project_id].firebaseio.co}////{projectId}/histories/{historyId}/executions/{executionId}/steps/{stepId}/perfSampleSeries/{sampleSeriesId}/samples
  tags: Sample Series
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/firebase/projectidhistorieshistoryidexecutionsexecutionidstepsstepidperfsampleseriessampleseriesidsamples-get-openapi.md
- name: Firebase Create Sample
  x-api-slug: firebase
  description: |-
    Creates a batch of PerfSamples - a client can submit multiple batches of Perf Samples through repeated calls to this method in order to split up a large request payload - duplicates and existing timestamp entries will be ignored. - the batch operation may partially succeed - the set of elements successfully inserted is returned in the response (omits items which already existed in the database).

    May return any of the following canonical error codes: - NOT_FOUND - The containing PerfSampleSeries does not exist
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://firebase.google.com/
  baseURL: https://{project_id].firebaseio.co}////{projectId}/histories/{historyId}/executions/{executionId}/steps/{stepId}/perfSampleSeries/{sampleSeriesId}/samples:batchCreate
  tags: Sample Series
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/firebase/projectidhistorieshistoryidexecutionsexecutionidstepsstepidperfsampleseriessampleseriesidsamplesbatchcreate-post-openapi.md
- name: Firebase
  x-api-slug: firebase
  description: Firebase is a mobile platform that helps you quicklydevelophigh-quality
    apps,growyour user base, andearnmore money. Firebase is made up of complementary
    features that you can mix-and-match to fit your needs.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://firebase.google.com/
  baseURL: https://{project_id].firebaseio.co}//
  tags: Series
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/firebase/openapi.md
x-common:
- type: x-blog
  url: https://firebase.googleblog.com/
- type: x-blog-rss
  url: http://firebase.googleblog.com/feeds/posts/default?alt=rss
- type: x-case-studies
  url: https://firebase.google.com/customers/
- type: x-change-log
  url: https://firebase.google.com/support/releases
- type: x-code
  url: https://firebase.google.com/docs/libraries/
- type: x-documentation
  url: https://firebase.google.com/docs/
- type: x-faq
  url: https://firebase.google.com/support/faq/
- type: x-forum
  url: https://groups.google.com/forum/#!forum/firebase-talk
- type: x-github
  url: https://github.com/firebase
- type: x-pricing
  url: https://firebase.google.com/pricing/
- type: x-pricing
  url: https://adwords.google.com/home/pricing/
- type: x-slack
  url: https://firebase.community/
- type: x-submit-bug
  url: https://firebase.google.com/support/contact/bugs-features
- type: x-support
  url: https://firebase.google.com/support/
- type: x-twitter
  url: https://twitter.com/firebase
- type: x-website
  url: https://firebase.google.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---