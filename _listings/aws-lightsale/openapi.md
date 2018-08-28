swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 1
info:
  title: AWS Lightsale API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetInstanceMetricData:
    get:
      summary: Get Instance Metric Data
      description: |-
        Returns the data points for the specified Amazon Lightsail instance metric, given an
              instance name.
      operationId: getInstanceMetricData
      x-api-path-slug: actiongetinstancemetricdata-get
      parameters:
      - in: query
        name: endTime
        description: The end time of the time period
        type: string
      - in: query
        name: instanceName
        description: The name of the instance for which you want to get metrics data
        type: string
      - in: query
        name: metricName
        description: The metric name to get data about
        type: string
      - in: query
        name: period
        description: The time period for which you are requesting data
        type: string
      - in: query
        name: startTime
        description: The start time of the time period
        type: string
      - in: query
        name: statistics
        description: The instance statistics
        type: string
      - in: query
        name: unit
        description: The unit
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances