---
name: BMC Software
x-slug: bmc-software
description: Transform your digital enterprise with BMC IT solutions. From mainframe
  to cloud to mobile, we???ll help you drive innovation and industrial efficiency.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
x-kinRank: "8"
x-alexaRank: "27308"
tags: Metrics
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/apis.md
specificationVersion: "0.14"
apis:
- name: BMC Software Merged API - Delete Mobile Device
  x-api-slug: v1mobiledevicesuserdeviceid-delete
  description: Deletes a device from a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Monitoring, Applications, Devops, SaaS, Enterprise, Technology, ISP, API Provider,
    API Service Provider, Profiles, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1mobiledevicesuserdeviceid-delete-openapi.md
- name: BMC Software Merged API - Create metric
  x-api-slug: v1metrics-post
  description: Creates a new metric
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Monitoring, Applications, Devops, SaaS, Enterprise, Technology, ISP, API Provider,
    API Service Provider, Profiles, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1metrics-post-openapi.md
- name: BMC Software Merged API - Get Metrics
  x-api-slug: v1metrics-get
  description: Retrieves the list of metrics in a project.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Monitoring, Applications, Devops, SaaS, Enterprise, Technology, ISP, API Provider,
    API Service Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1metrics-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1metrics-get-openapi.md
- name: BMC Software Merged API - Remove metric
  x-api-slug: v1metricsmetric-delete
  description: |-
    Removes a metric from the account.
     Note that a metric will not deleted if it has been alarmed unless that <em>removeAlarms</em>
     flag is added.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Monitoring, Applications, Devops, SaaS, Enterprise, Technology, ISP, API Provider,
    API Service Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1metricsmetric-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1metricsmetric-delete-openapi.md
- name: BMC Software Merged API - Get actions for a dashboard
  x-api-slug: v1metricsdashactionsdashboardsetid-get
  description: |-
    Retrieves the needed configuration changes for a dashboard
     Returns an an array of objects, each has the following properties:
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Monitoring, Applications, Devops, SaaS, Enterprise, Technology, ISP, API Provider,
    API Service Provider, Profiles, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1metricsdashactionsdashboardsetid-get-openapi.md
- name: BMC Software Merged API - Perform dashboard actions
  x-api-slug: v1metricsdashactionsdashboardsetid-post
  description: |-
    Performs necessary actions for a dashboard.
     Only enables or adds metrics at this time.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Monitoring, Applications, Devops, SaaS, Enterprise, Technology, ISP, API Provider,
    API Service Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1metricsdashactionsdashboardsetid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1metricsdashactionsdashboardsetid-post-openapi.md
- name: BMC Software Merged API - Update metric
  x-api-slug: v1metricsmetricname-put
  description: Updates a metric
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Monitoring, Applications, Devops, SaaS, Enterprise, Technology, ISP, API Provider,
    API Service Provider, Profiles, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/v1metricsmetricname-put-openapi.md
- name: BMC Software Merged API - Available metrics
  x-api-slug: metricsdefinitions-
  description: Determine which metrics are available to return historical data for,
    for a specific subject (device or service) over a specific time range.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Monitoring, Applications, Devops, SaaS, Enterprise, Technology, ISP, API Provider,
    API Service Provider, Profiles, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/metricsdefinitions--openapi.md
- name: BMC Software Merged API - Dynamic metrics
  x-api-slug: metricsdynamicgraphs-
  description: Return historical metrics data, for a devices and/or services that
    match a search or regex style inventory filter search over a specific time range.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Monitoring, Applications, Devops, SaaS, Enterprise, Technology, ISP, API Provider,
    API Service Provider, Profiles, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/bmc-software/metricsdynamicgraphs--openapi.md
x-common:
- type: x-api-gallery
  url: http://blogger.api.gallery.streamdata.io
- type: x-api-stack
  url: http://bmc.software.stack.network
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