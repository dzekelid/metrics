---
name: Firebase
x-slug: firebase
description: Firebase is a mobile platform that gives developers the tools and infrastructure
  to build better apps and grow successful businesses.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
x-kinRank: "9"
x-alexaRank: "1"
tags: Metrics
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/firebase/apis.md
specificationVersion: "0.14"
apis:
- name: Firebase Get Metrics Summary
  x-api-slug: firebase
  description: |-
    Retrieves a PerfMetricsSummary.

    May return any of the following error code(s): - NOT_FOUND - The specified PerfMetricsSummary does not exist
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}////{projectId}/histories/{historyId}/executions/{executionId}/steps/{stepId}/perfMetricsSummary
  tags: Metrics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/firebase/projectidhistorieshistoryidexecutionsexecutionidstepsstepidperfmetricssummary-get-openapi.md
- name: Firebase Create Metric Summary
  x-api-slug: firebase
  description: |-
    Creates a PerfMetricsSummary resource.

    May return any of the following error code(s): - ALREADY_EXISTS - A PerfMetricSummary already exists for the given Step - NOT_FOUND - The containing Step does not exist
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}////{projectId}/histories/{historyId}/executions/{executionId}/steps/{stepId}/perfMetricsSummary
  tags: Metrics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/firebase/projectidhistorieshistoryidexecutionsexecutionidstepsstepidperfmetricssummary-post-openapi.md
- name: Firebase
  x-api-slug: firebase
  description: Firebase is a mobile platform that gives developers the tools and infrastructure
    to build better apps and grow successful businesses.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}//
  tags: Metrics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/metrics/master/_listings/firebase/openapi.md
x-common:
- type: x-website
  url: https://Firebase.google.com
- type: x-blog
  url: https://firebase.googleblog.com/
- type: x-blog-rss
  url: http://firebase.googleblog.com/feeds/posts/default?alt=rss
- type: x-case-studies
  url: https://firebase.google.com/customers/
- type: x-change-log
  url: https://firebase.google.com/support/releases
- type: x-code
  url: https://firebase.google.com/docs/libraries/
- type: x-crunchbase
  url: https://crunchbase.com/organization/google
- type: x-documentation
  url: https://firebase.google.com/docs/
- type: x-faq
  url: https://firebase.google.com/support/faq/
- type: x-forum
  url: https://groups.google.com/forum/#!forum/firebase-talk
- type: x-github
  url: https://github.com/firebase
- type: x-pricing
  url: https://firebase.google.com/pricing/
- type: x-pricing
  url: https://adwords.google.com/home/pricing/
- type: x-slack
  url: https://firebase.community/
- type: x-submit-bug
  url: https://firebase.google.com/support/contact/bugs-features
- type: x-support
  url: https://firebase.google.com/support/
- type: x-twitter
  url: https://twitter.com/Google
- type: x-twitter
  url: https://twitter.com/firebase
- type: x-website
  url: https://firebase.google.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---