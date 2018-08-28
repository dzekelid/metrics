---
swagger: "2.0"
x-collection-name: Azure SQL Database
x-complete: 1
info:
  title: Azure SQL Database
  description: provides-create-read-update-and-delete-functionality-for-azure-sql-database-resources-including-servers-databases-elastic-pools-recommendations-operations-and-usage-metrics-
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/recommendedElasticPools/{recommendedElasticPoolName}/metrics
  : get:
      summary: Recommended Elastic Pools List Metrics
      description: Returns a recommented elastic pool metrics.
      operationId: RecommendedElasticPools_ListMetrics
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamerecommendedelasticpoolsrecommendedelasticpoolnamemetrics-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: recommendedElasticPoolName
        description: The name of the recommended elastic pool to be retrieved
      responses:
        200:
          description: OK
      tags:
      - Recommended Elastic Pools Metrics
---