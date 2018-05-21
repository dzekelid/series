---
swagger: "2.0"
x-collection-name: Firebase
x-complete: 1
info:
  title: Firebase
  description: you-can-use-any-firebase-database-url-as-a-rest-endpoint-all-you-need-to-do-is-append-json-to-the-end-of-the-url-and-send-a-request-from-your-favorite-https-client
  version: 1.0.0
host: '{project_id].firebaseio.co}'
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{projectId}/histories/{historyId}/executions/{executionId}/steps/{stepId}/perfSampleSeries:
    get:
      summary: Get Sample Series
      description: |-
        Lists PerfSampleSeries for a given Step.

        The request provides an optional filter which specifies one or more PerfMetricsType to include in the result; if none returns all. The resulting PerfSampleSeries are sorted by ids.

        May return any of the following canonical error codes: - NOT_FOUND - The containing Step does not exist
      operationId: toolresults.projects.histories.executions.steps.perfSampleSeries.list
      x-api-path-slug: projectidhistorieshistoryidexecutionsexecutionidstepsstepidperfsampleseries-get
      parameters:
      - in: path
        name: executionId
        description: A tool results execution ID
      - in: query
        name: filter
        description: Specify one or more PerfMetricType values such as CPU to filter
          the result
      - in: path
        name: historyId
        description: A tool results history ID
      - in: path
        name: projectId
        description: The cloud project
      - in: path
        name: stepId
        description: A tool results step ID
      responses:
        200:
          description: OK
      tags:
      - Sample Series
    post:
      summary: Create Sample Series
      description: |-
        Creates a PerfSampleSeries.

        May return any of the following error code(s): - ALREADY_EXISTS - PerfMetricSummary already exists for the given Step - NOT_FOUND - The containing Step does not exist
      operationId: toolresults.projects.histories.executions.steps.perfSampleSeries.create
      x-api-path-slug: projectidhistorieshistoryidexecutionsexecutionidstepsstepidperfsampleseries-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: executionId
        description: A tool results execution ID
      - in: path
        name: historyId
        description: A tool results history ID
      - in: path
        name: projectId
        description: The cloud project
      - in: path
        name: stepId
        description: A tool results step ID
      responses:
        200:
          description: OK
      tags:
      - Sample Series
  /{projectId}/histories/{historyId}/executions/{executionId}/steps/{stepId}/perfSampleSeries/{sampleSeriesId}:
    get:
      summary: Get Sample Series
      description: |-
        Gets a PerfSampleSeries.

        May return any of the following error code(s): - NOT_FOUND - The specified PerfSampleSeries does not exist
      operationId: toolresults.projects.histories.executions.steps.perfSampleSeries.get
      x-api-path-slug: projectidhistorieshistoryidexecutionsexecutionidstepsstepidperfsampleseriessampleseriesid-get
      parameters:
      - in: path
        name: executionId
        description: A tool results execution ID
      - in: path
        name: historyId
        description: A tool results history ID
      - in: path
        name: projectId
        description: The cloud project
      - in: path
        name: sampleSeriesId
        description: A sample series id
      - in: path
        name: stepId
        description: A tool results step ID
      responses:
        200:
          description: OK
      tags:
      - Sample Series
  /{projectId}/histories/{historyId}/executions/{executionId}/steps/{stepId}/perfSampleSeries/{sampleSeriesId}/samples:
    get:
      summary: Get Sample Series
      description: |-
        Lists the Performance Samples of a given Sample Series - The list results are sorted by timestamps ascending - The default page size is 500 samples; and maximum size allowed 5000 - The response token indicates the last returned PerfSample timestamp - When the results size exceeds the page size, submit a subsequent request including the page token to return the rest of the samples up to the page limit

        May return any of the following canonical error codes: - OUT_OF_RANGE - The specified request page_token is out of valid range - NOT_FOUND - The containing PerfSampleSeries does not exist
      operationId: toolresults.projects.histories.executions.steps.perfSampleSeries.samples.list
      x-api-path-slug: projectidhistorieshistoryidexecutionsexecutionidstepsstepidperfsampleseriessampleseriesidsamples-get
      parameters:
      - in: path
        name: executionId
        description: A tool results execution ID
      - in: path
        name: historyId
        description: A tool results history ID
      - in: query
        name: pageSize
        description: The default page size is 500 samples, and the maximum size is
          5000
      - in: query
        name: pageToken
        description: Optional, the next_page_token returned in the previous response
      - in: path
        name: projectId
        description: The cloud project
      - in: path
        name: sampleSeriesId
        description: A sample series id
      - in: path
        name: stepId
        description: A tool results step ID
      responses:
        200:
          description: OK
      tags:
      - Sample Series
  /{projectId}/histories/{historyId}/executions/{executionId}/steps/{stepId}/perfSampleSeries/{sampleSeriesId}/samples:batchCreate:
    post:
      summary: Create Sample
      description: |-
        Creates a batch of PerfSamples - a client can submit multiple batches of Perf Samples through repeated calls to this method in order to split up a large request payload - duplicates and existing timestamp entries will be ignored. - the batch operation may partially succeed - the set of elements successfully inserted is returned in the response (omits items which already existed in the database).

        May return any of the following canonical error codes: - NOT_FOUND - The containing PerfSampleSeries does not exist
      operationId: toolresults.projects.histories.executions.steps.perfSampleSeries.samples.batchCreate
      x-api-path-slug: projectidhistorieshistoryidexecutionsexecutionidstepsstepidperfsampleseriessampleseriesidsamplesbatchcreate-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: executionId
        description: A tool results execution ID
      - in: path
        name: historyId
        description: A tool results history ID
      - in: path
        name: projectId
        description: The cloud project
      - in: path
        name: sampleSeriesId
        description: A sample series id
      - in: path
        name: stepId
        description: A tool results step ID
      responses:
        200:
          description: OK
      tags:
      - Sample Series
---