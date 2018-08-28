---
swagger: "2.0"
x-collection-name: Google Analytics
x-complete: 0
info:
  title: Google Analytics Create Custom Metric
  description: Create a new custom metric.
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /analytics/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /management/accounts/{accountId}/webproperties/{webPropertyId}/customMetrics:
    get:
      summary: Get Custom Metrics
      description: Lists custom metrics to which the user has access.
      operationId: analytics.management.customMetrics.list
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustommetrics-get
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom metrics to retrieve
      - in: query
        name: max-results
        description: The maximum number of custom metrics to include in this response
      - in: query
        name: start-index
        description: An index of the first entity to retrieve
      - in: path
        name: webPropertyId
        description: Web property ID for the custom metrics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Metric
    post:
      summary: Create Custom Metric
      description: Create a new custom metric.
      operationId: analytics.management.customMetrics.insert
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustommetrics-post
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom metric to create
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: webPropertyId
        description: Web property ID for the custom dimension to create
      responses:
        200:
          description: OK
      tags:
      - Metric
  /management/accounts/{accountId}/webproperties/{webPropertyId}/customMetrics/{customMetricId}:
    get:
      summary: Get Custom Metric
      description: Get a custom metric to which the user has access.
      operationId: analytics.management.customMetrics.get
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustommetricscustommetricid-get
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom metric to retrieve
      - in: path
        name: customMetricId
        description: The ID of the custom metric to retrieve
      - in: path
        name: webPropertyId
        description: Web property ID for the custom metric to retrieve
      responses:
        200:
          description: OK
      tags:
      - Metric
    patch:
      summary: Update Custom Metric
      description: Updates an existing custom metric. This method supports patch semantics.
      operationId: analytics.management.customMetrics.patch
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustommetricscustommetricid-patch
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom metric to update
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customMetricId
        description: Custom metric ID for the custom metric to update
      - in: query
        name: ignoreCustomDataSourceLinks
        description: Force the update and ignore any warnings related to the custom
          metric being linked to a custom data source / data set
      - in: path
        name: webPropertyId
        description: Web property ID for the custom metric to update
      responses:
        200:
          description: OK
      tags:
      - Metric
    put:
      summary: Update Custom Metric
      description: Updates an existing custom metric.
      operationId: analytics.management.customMetrics.update
      x-api-path-slug: managementaccountsaccountidwebpropertieswebpropertyidcustommetricscustommetricid-put
      parameters:
      - in: path
        name: accountId
        description: Account ID for the custom metric to update
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customMetricId
        description: Custom metric ID for the custom metric to update
      - in: query
        name: ignoreCustomDataSourceLinks
        description: Force the update and ignore any warnings related to the custom
          metric being linked to a custom data source / data set
      - in: path
        name: webPropertyId
        description: Web property ID for the custom metric to update
      responses:
        200:
          description: OK
      tags:
      - Metric
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