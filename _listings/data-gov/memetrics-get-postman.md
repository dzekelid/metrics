{
  "info": {
    "name": "Data.gov API Get Me Metrics",
    "_postman_id": "de9e2f8d-99c2-4658-8b50-9cd93c477d2f",
    "description": "Fetch the current user (me) metrics",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "me",
      "item": [
        {
          "id": "5d69d310-989e-4984-b9cb-b40b73d0a77b",
          "name": "getMeMetrics",
          "request": {
            "url": "http://catalog.data.gov/api/3/me/metrics/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetch the current user (me) metrics"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "239cb5f2-b65b-48c9-8da5-7ca3b0b73309"
            }
          ]
        }
      ]
    }
  ]
}