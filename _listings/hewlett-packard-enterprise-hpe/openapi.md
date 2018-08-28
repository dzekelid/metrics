swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 1
info:
  title: HPE OneSphere API
  description: hpe-onesphere-hybrid-cloud-management-rest-api-for-calls-requiring-authentication-use-restsession-to-get-a-token-
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
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
      description: |-
        Returns all metrics based on the supplied criteria. It requires the **analyst** role.
        It requires one and only one of resourceUri or category to be specified.
      operationId: FindMetrics
      x-api-path-slug: metrics-get
      parameters:
      - in: query
        name: category
        description: A category name
      - in: query
        name: count
        description: Maximum number of response members to return
      - in: query
        name: groupBy
        description: A value to group the data by
      - in: query
        name: name
        description: Name(s) of metrics to return
      - in: query
        name: period
        description: How much time to cover per data point
      - in: query
        name: periodCount
        description: How many period data points to return relative to the periodStart
          time
      - in: query
        name: periodStart
        description: When the metric value(s) should be measured from
      - in: query
        name: query
        description: A query to filter the resources by
      - in: query
        name: resourceUri
        description: Resource(s) to return metrics for
      - in: query
        name: start
        description: Index into the response members to allow pagination
      - in: query
        name: view
        description: Whether to return related content
      responses:
        200:
          description: OK
      tags:
      - Metrics