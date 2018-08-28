swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 1
info:
  title: Broadleaf Commerce API
  description: the-default-broadleaf-commerce-apis
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /metrics:
    get:
      summary: Get Metrics
      description: Get metrics.
      operationId: getMetrics
      x-api-path-slug: metrics-get
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /metrics.json:
    get:
      summary: Get Metrics
      description: Get metrics.
      operationId: getMetrics.json
      x-api-path-slug: metrics-json-get
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /metrics/{name}:
    get:
      summary: Get Metrics Name
      description: Get metrics name.
      operationId: getMetricsName
      x-api-path-slug: metricsname-get
      parameters:
      - in: path
        name: name
        description: name
      responses:
        200:
          description: OK
      tags:
      - Metrics
      - Name