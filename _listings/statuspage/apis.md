---
name: StatusPage
x-slug: statuspage
description: StatusPage.io is the best way for web infrastructure, developer API,
  and SaaS companies to get set up with their very own status page in minutes
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18898-statuspage-io.jpg
x-kinRank: "8"
x-alexaRank: "34303"
tags: Metrics
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/statuspage/apis.md
specificationVersion: "0.14"
apis:
- name: StatusPage.io Get a list of available public metric providers
  x-api-slug: statuspage-io
  description: Get a list of available public metric providers
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18898-statuspage-io.jpg
  humanURL: https://www.statuspage.io/
  baseURL: https://///metrics_providers.json
  tags: Metrics
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/statuspage/metrics-providers-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/statuspage/metrics-providers-json-get-openapi.md
- name: StatusPage.io Submit data for a custom metric
  x-api-slug: statuspage-io
  description: Submit data for a custom metric
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18898-statuspage-io.jpg
  humanURL: https://www.statuspage.io/
  baseURL: https://///pages/[page_id]/metrics/[metric_id]/data.json
  tags: Metrics
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/statuspage/pagespage-idmetricsmetric-iddata-json-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/statuspage/pagespage-idmetricsmetric-iddata-json-post-openapi.md
- name: StatusPage.io Delete all data for a custom metric
  x-api-slug: statuspage-io
  description: Delete all data for a custom metric
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18898-statuspage-io.jpg
  humanURL: https://www.statuspage.io/
  baseURL: https://///pages/[page_id]/metrics/[metric_id]/data.json
  tags: Metrics
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/statuspage/pagespage-idmetricsmetric-iddata-json-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/statuspage/pagespage-idmetricsmetric-iddata-json-delete-openapi.md
- name: StatusPage.io
  x-api-slug: statuspage-io
  description: StatusPage.io is the best way for web infrastructure, developer API,
    and SaaS companies to get set up with their very own status page in minutes
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18898-statuspage-io.jpg
  humanURL: https://www.statuspage.io/
  baseURL: https:///
  tags: Metrics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/statuspage/openapi.md
x-common:
- type: x-authentication
  url: http://doers.statuspage.io/api/authentication/
- type: x-blog
  url: http://blog.statuspage.io
- type: x-blog-rss
  url: http://blog.statuspage.io/posts.rss
- type: x-crunchbase
  url: https://crunchbase.com/organization/statuspage
- type: x-developer
  url: http://doers.statuspage.io/
- type: x-email
  url: hi@statuspage.io
- type: x-github
  url: https://github.com/statuspage
- type: x-pricing
  url: https://www.statuspage.io/pricing
- type: x-privacy
  url: https://www.statuspage.io/privacy-policy
- type: x-security
  url: https://www.statuspage.io/security
- type: x-status
  url: http://metastatuspage.com/
- type: x-terms-of-service
  url: https://www.statuspage.io/terms-of-service
- type: x-twitter
  url: https://twitter.com/statuspageio
- type: x-website
  url: https://www.statuspage.io/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---