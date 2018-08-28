swagger: "2.0"
x-collection-name: AWS S3
x-complete: 1
info:
  title: No Title
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?metrics:
    get:
      summary: List Bucket Metrics
      description: Lists the metrics configurations for the CloudWatch request metrics
        of the bucket
      operationId: list-bucket-metrics
      x-api-path-slug: metrics-get
      parameters:
      - in: query
        name: BucketName
        description: The name of the bucket containing the metrics configurationstttttttttto
          retrieve
      - in: query
        name: ContinuationToken
        description: The marker that is used to continue a metrics configurationtttttttttlisting
          that has been truncated
      responses:
        200:
          description: OK
      tags:
      - List
      - Bucket
      - Metrics
  /?metrics&amp;id=Id:
    delete:
      summary: DELETE Bucket Metrics
      description: Deletes a metrics configuration for the CloudWatch request metrics
        (specified by the metricsconfiguration ID) from the bucket
      operationId: delete-bucket-metrics
      x-api-path-slug: metricsampidid-delete
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Metrics
    put:
      summary: PUT Bucket Metrics
      description: Sets or updates a metrics configuration for the CloudWatch request
        metrics (specified by themetrics configuration ID) from the bucket
      operationId: put-bucket-metrics
      x-api-path-slug: metricsampidid-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Metrics
  /?metrics&amp;id=id:
    get:
      summary: GET Bucket Metrics
      description: Gets a metrics configuration for the CloudWatch request metrics
        (specified by the metricsconfiguration ID) from the bucket
      operationId: get-bucket-metrics
      x-api-path-slug: metricsampidid-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Metrics