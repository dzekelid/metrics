---
swagger: "2.0"
x-collection-name: IBM Watson
x-complete: 0
info:
  title: IBM Watson Machine Learning Get Wml Instances Instance Published Models Published
    Model Evaluation Metrics
  description: Get wml instances instance published models published model evaluation
    metrics.
  version: 1.0.0
host: ibm-watson-ml.mybluemix.net
basePath: v3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /wml_instances/{instance_id}/published_models/{published_model_id}/evaluation_metrics:
    get:
      summary: Get Wml Instances Instance Published Models Published Model Evaluation
        Metrics
      description: Get wml instances instance published models published model evaluation
        metrics.
      operationId: listModelMetrics
      x-api-path-slug: wml-instancesinstance-idpublished-modelspublished-model-idevaluation-metrics-get
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Wml
      - Instances
      - Instance
      - Id
      - Published
      - Models
      - Published
      - Model
      - Id
      - Evaluation
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