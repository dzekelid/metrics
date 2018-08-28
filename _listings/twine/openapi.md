swagger: "2.0"
x-collection-name: Twine
x-complete: 1
info:
  title: Twine
  description: -overviewthe-twine-health-api-is-restful-api--the-requests-and-responses-are-formated-according-to-the-json-apihttpjsonapi-orgformat1-0-specification-in-addition-to-this-documentation-we-also-provide-an-openapihttpsgithub-comoaiopenapispecificationblobmasterversions2-0-md-yaml-file-describing-the-api-twine-api-specificationswagger-yaml--authenticationauthentication-for-the-twine-api-is-based-on-the-oauth-2-0-authorization-frameworkhttpstools-ietf-orghtmlrfc6749--twine-currently-supports-grant-types-of-client-credentials-and-refresh-token-see-post-oauthtokenoperationcreatetoken-for-details-on-the-request-and-response-formats--redocinject-securitydefinitions-
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