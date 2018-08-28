---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Get Sekiq Queue Metrics
  version: 1.0.0
  description: Get the Sidekiq queue metrics
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/sidekiq/queue_metrics:
    get:
      summary: Get Sekiq Queue Metrics
      description: Get the Sidekiq queue metrics
      operationId: getV3SidekiqQueueMetrics
      x-api-path-slug: v3sidekiqqueue-metrics-get
      responses:
        200:
          description: OK
      tags:
      - Sekiq
      - Queue
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