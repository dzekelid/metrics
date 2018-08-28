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
  /?Action=PutMetricAlarm:
    "":
      summary: Put Metric Alarm
      description: Creates or updates an alarm and associates it with the specified
        metric.
      operationId: putmetricalarm
      x-api-path-slug: actionputmetricalarm-
      parameters:
      - in: query
        name: ActionsEnabled
        description: Indicates whether actions should be executed during any changes
          to the alarm state
        type: string
      - in: query
        name: AlarmActions.member.N
        description: The actions to execute when this alarm transitions to the ALARM
          state from any other state
        type: string
      - in: query
        name: AlarmDescription
        description: The description for the alarm
        type: string
      - in: query
        name: AlarmName
        description: The name for the alarm
        type: string
      - in: query
        name: ComparisonOperator
        description: The arithmetic operation to use when comparing the specified
          statistic andthreshold
        type: string
      - in: query
        name: Dimensions.member.N
        description: The dimensions for the metric associated with the alarm
        type: string
      - in: query
        name: EvaluationPeriods
        description: The number of periods over which data is compared to the specifiedthreshold
        type: string
      - in: query
        name: ExtendedStatistic
        description: The percentile statistic for the metric associated with the alarm
        type: string
      - in: query
        name: InsufficientDataActions.member.N
        description: The actions to execute when this alarm transitions to the INSUFFICIENT_DATA
          state from any other state
        type: string
      - in: query
        name: MetricName
        description: The name for the metric associated with the alarm
        type: string
      - in: query
        name: Namespace
        description: The namespace for the metric associated with the alarm
        type: string
      - in: query
        name: OKActions.member.N
        description: The actions to execute when this alarm transitions to an OK statefrom
          any other state
        type: string
      - in: query
        name: Period
        description: The period, in seconds, over which the specified statistic is
          applied
        type: string
      - in: query
        name: Statistic
        description: The statistic for the metric associated with the alarm, other
          than percentile
        type: string
      - in: query
        name: Threshold
        description: The value against which the specified statistic is compared
        type: string
      - in: query
        name: Unit
        description: The unit of measure for the statistic
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarm Metric
  /?Action=PutMetricData:
    "":
      summary: Put Metric Data
      description: Publishes metric data points to Amazon CloudWatch.
      operationId: putmetricdata
      x-api-path-slug: actionputmetricdata-
      parameters:
      - in: query
        name: MetricData.member.N
        description: The data for the metric
        type: string
      - in: query
        name: Namespace
        description: The namespace for the metric data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Data Metric