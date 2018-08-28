{
  "info": {
    "name": "Azure IoT Hub API Iot Hub Resource Get Quota Metrics",
    "_postman_id": "0927d09e-8a7e-4805-8ea7-4af44d136ffa",
    "description": "Get the quota metrics for an IoT hub.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "iot hub resource quota metrics",
      "item": [
        {
          "id": "fd0f6ec1-7009-45a7-981c-42f41fa5bfd7",
          "name": "IotHubResource_GetQuotaMetrics",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Devices/IotHubs/:resourceName/quotaMetrics"
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
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the quota metrics for an IoT hub"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58f01734-7b08-40d4-b257-3cb7f5a41000"
            }
          ]
        }
      ]
    }
  ]
}