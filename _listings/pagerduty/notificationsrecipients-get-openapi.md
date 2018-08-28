---
swagger: "2.0"
x-collection-name: PagerDuty
x-complete: 0
info:
  title: PagerDuty Creating a recipient
  version: 1.0.0
  description: Create recipients for your alert notifications
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /notifications/recipients:
    get:
      summary: Creating a recipient
      description: Create recipients for your alert notifications
      operationId: creating-a-recipient
      x-api-path-slug: notificationsrecipients-get
      parameters:
      - in: body
        name: channel
        description: Channel name for chat integrations
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: name
        description: The name of your notification integration
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: token
        description: Your integration API token
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: type
        description: The type of notification integration
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: url
        description: URL for webhook integrations
        schema:
          $ref: '#/definitions/holder'
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