---
swagger: "2.0"
x-collection-name: AWS CloudWatch
x-complete: 1
info:
  title: AWS CloudWatch API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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
---