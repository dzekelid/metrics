---
name: BMC Software
x-slug: bmc-software
description: Transform your digital enterprise with BMC IT solutions. From mainframe
  to cloud to mobile, we???ll help you drive innovation and industrial efficiency.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
x-kinRank: "8"
x-alexaRank: "27308"
tags: Metrics
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/apis.md
specificationVersion: "0.14"
apis:
- name: BMC Software API Delete Mobile Device
  x-api-slug: bmc-software-api
  description: Deletes a device from a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/mobile-devices/:userDeviceId
  tags: Metrics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1mobiledevicesuserdeviceid-delete-openapi.md
- name: BMC Software API Create metric
  x-api-slug: bmc-software-api
  description: Creates a new metric
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/metrics
  tags: Metrics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1metrics-post-openapi.md
- name: BMC Software API Get Metrics
  x-api-slug: bmc-software-api
  description: Retrieves the list of metrics in a project.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/metrics
  tags: Metrics
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1metrics-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1metrics-get-openapi.md
- name: BMC Software API Remove metric
  x-api-slug: bmc-software-api
  description: |-
    Removes a metric from the account.
     Note that a metric will not deleted if it has been alarmed unless that <em>removeAlarms</em>
     flag is added.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/metrics/:metric
  tags: Metrics
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1metricsmetric-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1metricsmetric-delete-openapi.md
- name: BMC Software API Get actions for a dashboard
  x-api-slug: bmc-software-api
  description: |-
    Retrieves the needed configuration changes for a dashboard
     Returns an an array of objects, each has the following properties:
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/metrics/dashactions/:dashboardSetId
  tags: Metrics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1metricsdashactionsdashboardsetid-get-openapi.md
- name: BMC Software API Perform dashboard actions
  x-api-slug: bmc-software-api
  description: |-
    Performs necessary actions for a dashboard.
     Only enables or adds metrics at this time.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/metrics/dashactions/:dashboardSetId
  tags: Metrics
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1metricsdashactionsdashboardsetid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1metricsdashactionsdashboardsetid-post-openapi.md
- name: BMC Software API Update metric
  x-api-slug: bmc-software-api
  description: Updates a metric
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/metrics/:metricName
  tags: Metrics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1metricsmetricname-put-openapi.md
- name: BMC Software API Available metrics
  x-api-slug: bmc-software-api
  description: Determine which metrics are available to return historical data for,
    for a specific subject (device or service) over a specific time range.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///metrics/definitions
  tags: Metrics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/metricsdefinitions--openapi.md
- name: BMC Software API Dynamic metrics
  x-api-slug: bmc-software-api
  description: Return historical metrics data, for a devices and/or services that
    match a search or regex style inventory filter search over a specific time range.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///metrics/dynamicgraphs/
  tags: Metrics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/metricsdynamicgraphs--openapi.md
- name: BMC Software API
  x-api-slug: bmc-software-api
  description: Transform your digital enterprise with BMC IT solutions. From mainframe
    to cloud to mobile, we???ll help you drive innovation and industrial efficiency.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Metrics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/openapi.md
x-common:
- type: x-blog
  url: http://www.bmc.com/blogs
- type: x-blog-rss
  url: http://feeds.feedburner.com/BmcBlogs
- type: x-crunchbase
  url: https://crunchbase.com/organization/bmc
- type: x-documentation
  url: https://docs.bmc.com/docs/dashboard.action
- type: x-email
  url: customer_support@bmc.com
- type: x-email
  url: NA_Accounts_Payable@bmc.com
- type: x-email
  url: Collections_NA@bmc.com
- type: x-email
  url: education@bmc.com
- type: x-email
  url: investor@bmc.com
- type: x-email
  url: global_security@bmc.com
- type: x-email
  url: Compliance_EthicsOffice@bmc.com
- type: x-email
  url: 26Ethics@bmc.com
- type: x-email
  url: Community_Relations@bmc.com
- type: x-github
  url: https://github.com/bmcsoftware
- type: x-twitter
  url: https://twitter.com/bmcsoftware
- type: x-website
  url: http://www.bmc.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---