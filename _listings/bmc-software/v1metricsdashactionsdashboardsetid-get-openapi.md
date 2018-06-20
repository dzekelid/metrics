---
swagger: "2.0"
x-collection-name: BMC Software
x-complete: 0
info:
  title: BMC Software API Get actions for a dashboard
  version: 1.0.0
  description: |-
    Retrieves the needed configuration changes for a dashboard
     Returns an an array of objects, each has the following properties:
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