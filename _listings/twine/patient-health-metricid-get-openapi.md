---
swagger: "2.0"
x-collection-name: Twine
x-complete: 0
info:
  title: Twine Get a patient health metric
  description: Get the plan summary for a patient.
  version: 7.18.0
host: api.twinehealth.com
basePath: /pub
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /patient_health_metric:
    get:
      summary: List patient health metrics
      description: Get a list of patient health metrics.
      operationId: fetchPatientHealthMetrics
      x-api-path-slug: patient-health-metric-get
      parameters:
      - in: query
        name: filter[patient]
        description: Filter the patient health metrics for a specified patient
      - in: query
        name: page[number]
        description: Page number
      - in: query
        name: page[size]
        description: Page size
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Patient
      - Health
      - Metrics
    post:
      summary: Create patient health metrics
      description: |-
        Create one or more patient health metrics.

        Example for creating a patient health result with a patient specified using `meta.query` instead of `id`:

        ```JSON
          {
            "data": {
              "type": "patient_health_metric",
               "attributes": {
                 "code": {
                   "system": "LOINC",
                   "value": "13457-7"
                 },
                 "type": "ldl_cholesterol",
                 "occurred_at": "2017-03-14T11:00:57.000Z",
                 "value": "121",
                 "unit": "mg/dl"
              },
              "relationships": {
                "patient": {
                  "data": {
                    "type": "patient",
                    "meta": {
                      "query": {
                        "identifier": {
                          "system": "medical-record-number",
                          "value": "121212"
                        },
                        "organization": "58c4554710123c5c40dbab81"
                      }
                    }
                  }
                }
              }
            }
          }
        ```
      operationId: createPatientHealthMetric
      x-api-path-slug: patient-health-metric-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Patient
      - Health
      - Metrics
  /patient_health_metric/{id}:
    get:
      summary: Get a patient health metric
      description: Get the plan summary for a patient.
      operationId: fetchPatientHealthMetric
      x-api-path-slug: patient-health-metricid-get
      parameters:
      - in: path
        name: id
        description: Patient health metric identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Patient
      - Health
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