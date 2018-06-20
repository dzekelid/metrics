{
  "info": {
    "name": "Runscope Get Buckets Tests Metrics",
    "_postman_id": "2eea5240-ca25-45f3-8446-78da5bb2b9fc",
    "description": "Return details of the test metrics for the specified timeframe.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "buckets",
      "item": [
        {
          "id": "6baeac2f-b07b-49ec-84e3-d8d316dc4a14",
          "name": "buckets.bucketKey.tests.testId.metrics.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.runscope.com",
              "path": [
                "buckets/:bucketKey/tests/:testId/metrics"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "bucketKey",
                  "value": "bucketKey",
                  "type": "string"
                },
                {
                  "id": "testId",
                  "value": "testId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return details of the test metrics for the specified timeframe"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e878a24-23dc-4c11-95df-4745d2152d80"
            }
          ]
        }
      ]
    }
  ]
}