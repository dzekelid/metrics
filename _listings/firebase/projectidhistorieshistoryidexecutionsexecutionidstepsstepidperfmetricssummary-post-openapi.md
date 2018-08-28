---
swagger: "2.0"
x-collection-name: Firebase
x-complete: 0
info:
  title: Firebase Create Metric Summary
  description: |-
    Creates a PerfMetricsSummary resource.

    May return any of the following error code(s): - ALREADY_EXISTS - A PerfMetricSummary already exists for the given Step - NOT_FOUND - The containing Step does not exist
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
  /{projectId}/histories/{historyId}/executions/{executionId}/steps/{stepId}/perfMetricsSummary:
    get:
      summary: Get Metrics Summary
      description: |-
        Retrieves a PerfMetricsSummary.

        May return any of the following error code(s): - NOT_FOUND - The specified PerfMetricsSummary does not exist
      operationId: toolresults.projects.histories.executions.steps.getPerfMetricsSummary
      x-api-path-slug: projectidhistorieshistoryidexecutionsexecutionidstepsstepidperfmetricssummary-get
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
        name: stepId
        description: A tool results step ID
      responses:
        200:
          description: OK
      tags:
      - Metrics
    post:
      summary: Create Metric Summary
      description: |-
        Creates a PerfMetricsSummary resource.

        May return any of the following error code(s): - ALREADY_EXISTS - A PerfMetricSummary already exists for the given Step - NOT_FOUND - The containing Step does not exist
      operationId: toolresults.projects.histories.executions.steps.perfMetricsSummary.create
      x-api-path-slug: projectidhistorieshistoryidexecutionsexecutionidstepsstepidperfmetricssummary-post
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
      - Metrics
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