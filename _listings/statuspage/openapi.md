---
swagger: "2.0"
x-collection-name: StatusPage
x-complete: 1
info:
  title: StatusPage.io
  version: 1.0.0
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
    delete:
      summary: Delete all data for a custom metric
      description: Delete all data for a custom metric
      operationId: delete-all-data-for-a-custom-metric
      x-api-path-slug: pagespage-idmetricsmetric-iddata-json-delete
      responses:
        200:
          description: OK
      tags:
      - Metrics
---