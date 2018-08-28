{
  "info": {
    "name": "Azure SQL Database API Recommended Elastic Pools List Metrics",
    "_postman_id": "2b86dd7d-c1e9-4365-8527-199e8bea4c9f",
    "description": "Returns a recommented elastic pool metrics.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "recommended elastic pools metrics",
      "item": [
        {
          "id": "91fd0328-7727-4168-be97-ee9560c366e5",
          "name": "RecommendedElasticPools_ListMetrics",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/recommendedElasticPools/:recommendedElasticPoolName/metrics"
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
                  "id": "recommendedElasticPoolName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                },
                {
                  "id": "serverName",
                  "value": "serverName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a recommented elastic pool metrics"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42a4cdbd-18aa-4eeb-a031-faf89a769e3d"
            }
          ]
        }
      ]
    }
  ]
}