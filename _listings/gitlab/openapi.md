swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
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
  /v3/sidekiq/process_metrics:
    get:
      summary: Get Sekiq Process Metrics
      description: Get the Sidekiq process metrics
      operationId: getV3SidekiqProcessMetrics
      x-api-path-slug: v3sidekiqprocess-metrics-get
      responses:
        200:
          description: OK
      tags:
      - Sekiq
      - Process
      - Metrics
  /v3/sidekiq/compound_metrics:
    get:
      summary: Get Sekiq Compound Metrics
      description: Get the Sidekiq Compound metrics. Includes queue, process, and
        job statistics
      operationId: getV3SidekiqCompoundMetrics
      x-api-path-slug: v3sidekiqcompound-metrics-get
      responses:
        200:
          description: OK
      tags:
      - Sekiq
      - Compound
      - Metrics