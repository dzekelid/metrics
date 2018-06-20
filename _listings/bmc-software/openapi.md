---
swagger: "2.0"
x-collection-name: BMC Software
x-complete: 1
info:
  title: BMC Software Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/mobile-devices/:userDeviceId:
    delete:
      summary: Delete Mobile Device
      description: Deletes a device from a user
      operationId: delete-mobile-device
      x-api-path-slug: v1mobiledevicesuserdeviceid-delete
      parameters:
      - in: query
        name: |-
          userDeviceId
          The user device ID to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /v1/metrics:
    post:
      summary: Create metric
      description: Creates a new metric
      operationId: create-metric
      x-api-path-slug: v1metrics-post
      parameters:
      - in: formData
        name: |-
          name
          Name of the metric, must be globally unique, recommended that you add your own namespace
        description: typeType of metric, could be a device metric, a plugin metric
          or any arbitrary type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Metrics
    get:
      summary: Get Metrics
      description: Retrieves the list of metrics in a project.
      operationId: get-metrics
      x-api-path-slug: v1metrics-get
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /v1/metrics/:metric:
    delete:
      summary: Remove metric
      description: |-
        Removes a metric from the account.
         Note that a metric will not deleted if it has been alarmed unless that <em>removeAlarms</em>
         flag is added.
      operationId: remove-metric
      x-api-path-slug: v1metricsmetric-delete
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /v1/metrics/dashactions/:dashboardSetId:
    get:
      summary: Get actions for a dashboard
      description: |-
        Retrieves the needed configuration changes for a dashboard
         Returns an an array of objects, each has the following properties:
      operationId: get-actions-for-a-dashboard
      x-api-path-slug: v1metricsdashactionsdashboardsetid-get
      responses:
        200:
          description: OK
      tags:
      - Metrics
    post:
      summary: Perform dashboard actions
      description: |-
        Performs necessary actions for a dashboard.
         Only enables or adds metrics at this time.
      operationId: perform-dashboard-actions
      x-api-path-slug: v1metricsdashactionsdashboardsetid-post
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /v1/metrics/:metricName:
    put:
      summary: Update metric
      description: Updates a metric
      operationId: update-metric
      x-api-path-slug: v1metricsmetricname-put
      parameters:
      - in: formData
        name: |-
          type
          Type of metric, could be a device metric, a plugin metric or any arbitrary type
        description: descriptionDescription of the metric
        type: string
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /metrics/definitions:
    "":
      summary: Available metrics
      description: Determine which metrics are available to return historical data
        for, for a specific subject (device or service) over a specific time range.
      operationId: available-metrics
      x-api-path-slug: metricsdefinitions-
      parameters:
      - in: query
        name: end
        description: The UTC date string for the end time range in format YYYY-MM-DDTHH:mm:SSZ
          e
        type: string
      - in: query
        name: start
        description: The UTC date string for the start time range in format YYYY-MM-DDTHH:mm:SSZ
          e
        type: string
      - in: query
        name: subjectId
        description: The ID of the subject to get the definitions for, e
        type: string
      - in: query
        name: token
        description: Your API token
        type: string
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /metrics/dynamicgraphs/:
    "":
      summary: Dynamic metrics
      description: Return historical metrics data, for a devices and/or services that
        match a search or regex style inventory filter search over a specific time
        range.
      operationId: dynamic-metrics
      x-api-path-slug: metricsdynamicgraphs-
      parameters:
      - in: query
        name: end
        description: The UTC date string for the end time range in format YYYY-MM-DDTHH:mm:SSZ
          e
        type: string
      - in: query
        name: ids
        description: List of inventory IDs
        type: string
      - in: query
        name: inventoryFilter
        description: A regular expression that will return all devices or services
          that match the pattern
        type: string
      - in: query
        name: names
        description: Human-readable names of a device or service
        type: string
      - in: query
        name: start
        description: The UTC date string for the start time range in format YYYY-MM-DDTHH:mm:SSZ
          e
        type: string
      - in: query
        name: token
        description: Your API token
        type: string
      - in: query
        name: type
        description: Specify whether to return only devices, services or all
        type: string
      responses:
        200:
          description: OK
      tags:
      - Metrics
---