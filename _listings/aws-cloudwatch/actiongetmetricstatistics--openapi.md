---
swagger: "2.0"
x-collection-name: AWS CloudWatch
x-complete: 0
info:
  title: Amazon CloudWatch API Get Metric Statistics
  version: 1.0.0
  description: Gets statistics for the specified metric.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListMetrics:
    "":
      summary: List Metrics
      description: List the specified metrics.
      operationId: listmetrics
      x-api-path-slug: actionlistmetrics-
      parameters:
      - in: query
        name: Dimensions.member.N
        description: The dimensions to filter against
        type: string
      - in: query
        name: MetricName
        description: The name of the metric to filter against
        type: string
      - in: query
        name: Namespace
        description: The namespace to filter against
        type: string
      - in: query
        name: NextToken
        description: The token returned by a previous call to indicate that there
          is more dataavailable
        type: string
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /?Action=DescribeAlarmsForMetric:
    "":
      summary: Describe Alarms For Metric
      description: Retrieves the alarms for the specified metric.
      operationId: describealarmsformetric
      x-api-path-slug: actiondescribealarmsformetric-
      parameters:
      - in: query
        name: Dimensions.member.N
        description: The dimensions associated with the metric
        type: string
      - in: query
        name: ExtendedStatistic
        description: The percentile statistic for the metric
        type: string
      - in: query
        name: MetricName
        description: The name of the metric
        type: string
      - in: query
        name: Namespace
        description: The namespace of the metric
        type: string
      - in: query
        name: Period
        description: The period, in seconds, over which the statistic is applied
        type: string
      - in: query
        name: Statistic
        description: The statistic for the metric, other than percentiles
        type: string
      - in: query
        name: Unit
        description: The unit for the metric
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarm Metrics
  /?Action=GetMetricStatistics:
    "":
      summary: Get Metric Statistics
      description: Gets statistics for the specified metric.
      operationId: getmetricstatistics
      x-api-path-slug: actiongetmetricstatistics-
      parameters:
      - in: query
        name: Dimensions.member.N
        description: The dimensions
        type: string
      - in: query
        name: EndTime
        description: The time stamp that determines the last data point to return
        type: string
      - in: query
        name: ExtendedStatistics.member.N
        description: The percentile statistics
        type: string
      - in: query
        name: MetricName
        description: The name of the metric, with or without spaces
        type: string
      - in: query
        name: Namespace
        description: The namespace of the metric, with or without spaces
        type: string
      - in: query
        name: Period
        description: The granularity, in seconds, of the returned data points
        type: string
      - in: query
        name: StartTime
        description: The time stamp that determines the first data point to return
        type: string
      - in: query
        name: Statistics.member.N
        description: The metric statistics, other than percentile
        type: string
      - in: query
        name: Unit
        description: The unit for a given metric
        type: string
      responses:
        200:
          description: OK
      tags:
      - Metric Statistics
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