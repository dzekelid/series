---
name: DataDog
x-slug: datadog
description: Datadog is a monitoring service that brings together metrics and events
  from servers, databases, applications, tools and services to present a unified view
  of the infrastructure. These capabilities are provided on a SaaS-based data analytics
  platform that enables Dev and Ops teams to work collaboratively on the infrastructure
  to avoid downtime, resolve performance problems, and ensure that development and
  deployment cycles finish on time.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/datadog-logo.png
x-kinRank: "8"
x-alexaRank: ""
tags: Series
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/datadog/apis.md
specificationVersion: "0.14"
apis:
- name: DataDog API Add Series
  x-api-slug: datadog-api
  description: |-
    The metrics end-point allows you to post time-series data that can be
              graphed on Datadog's dashboards.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/datadog-logo.png
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1///series
  tags: Monitoring,Series
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/datadog/series-post-openapi.md
- name: DataDog API
  x-api-slug: datadog-api
  description: Datadog is a monitoring service that brings together metrics and events
    from servers, databases, applications, tools and services to present a unified
    view of the infrastructure. These capabilities are provided on a SaaS-based data
    analytics platform that enables Dev and Ops teams to work collaboratively on the
    infrastructure to avoid downtime, resolve performance problems, and ensure that
    development and deployment cycles finish on time.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/datadog-logo.png
  humanURL: https://www.datadoghq.com/
  baseURL: https:///api/v1/
  tags: Series
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/datadog/openapi.md
x-common:
- type: x-blog
  url: https://www.datadoghq.com/blog/
- type: x-blog-rss
  url: https://www.datadoghq.com/feed/
- type: x-github
  url: https://github.com/datadog
- type: x-twitter
  url: https://twitter.com/datadoghq
- type: x-integrations
  url: https://www.datadoghq.com/product/integrations/
- type: x-pricing
  url: https://www.datadoghq.com/pricing/
- type: x-security
  url: https://www.datadoghq.com/security/
- type: x-website
  url: https://www.datadoghq.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---