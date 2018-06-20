---
swagger: "2.0"
x-collection-name: StatusPage.io
x-complete: 0
info:
  title: StatusPage.io Submit data for a custom metric
  version: 1.0.0
  description: Submit data for a custom metric
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /metrics_providers.json:
    get:
      summary: Get a list of available public metric providers
      description: Get a list of available public metric providers
      operationId: get-a-list-of-available-public-metric-providers
      x-api-path-slug: metrics-providers-json-get
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /pages/[page_id]/metrics/[metric_id]/data.json:
    post:
      summary: Submit data for a custom metric
      description: Submit data for a custom metric
      operationId: submit-data-for-a-custom-metric
      x-api-path-slug: pagespage-idmetricsmetric-iddata-json-post
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