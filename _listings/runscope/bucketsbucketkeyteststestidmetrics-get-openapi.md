---
swagger: "2.0"
x-collection-name: Runscope
x-complete: 0
info:
  title: Runscope Get Buckets Tests Metrics
  description: Return details of the test metrics for the specified timeframe.
  version: 1.0.0
host: api.runscope.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /buckets/{bucketKey}/tests/{testId}/metrics:
    get:
      summary: Get Buckets Tests Metrics
      description: Return details of the test metrics for the specified timeframe.
      operationId: buckets.bucketKey.tests.testId.metrics.get
      x-api-path-slug: bucketsbucketkeyteststestidmetrics-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
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