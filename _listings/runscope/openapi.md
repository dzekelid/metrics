---
swagger: "2.0"
x-collection-name: Runscope
x-complete: 1
info:
  title: Runscope
  description: manage-runscope-programmatically-
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
---