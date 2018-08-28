---
name: Predix
x-slug: predix
description: Predix (IoT PaaS) helps you develop apps that connect people with industrial
  machines through analytics and data for better business outcomes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
x-kinRank: "7"
x-alexaRank: "264121"
tags: Existing
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/existing/master/_listings/predix/apis.md
specificationVersion: "0.14"
apis:
- name: Access Control - Creates a list of resources for the given zone. Existing
    resources will be updated with the provided values.
  x-api-slug: v1resource-post
  description: Creates a list of resources for the given zone. existing resources
    will be updated with the provided values..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https://predix-acs.run.aws-usw02-pr.ice.predix.io//
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/existing/master/_listings/predix/v1resource-post-openapi.md
- name: Access Control - Creates a list of subjects. Existing subjects will be updated
    with the provided values.
  x-api-slug: v1subject-post
  description: Creates a list of subjects. existing subjects will be updated with
    the provided values..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https://predix-acs.run.aws-usw02-pr.ice.predix.io//
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/existing/master/_listings/predix/v1subject-post-openapi.md
- name: Analytics Framework - Update an existing scheduler job.
  x-api-slug: apiv1schedulerjobsid-put
  description: Updates the scheduled job. The updated changes will be effective from
    the next scheduling of this job. To suspend a job, update the job with state value
    'Inactive'. To resume a job, update the job with state value 'Active'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/existing/master/_listings/predix/apiv1schedulerjobsid-put-openapi.md
- name: Analytics Framework - Update an existing orchestration configuration entry.
  x-api-slug: apiv2configorchestrationsid-put
  description: Updates the orchestration configuration entry with given orchestration
    configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/existing/master/_listings/predix/apiv2configorchestrationsid-put-openapi.md
- name: Analytics Runtime - Update an existing scheduler job.
  x-api-slug: apiv1schedulerjobsid-put
  description: Updates the scheduled job. The updated changes will be effective from
    the next scheduling of this job. To suspend a job, update the job with state value
    'Inactive'. To resume a job, update the job with state value 'Active'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/existing/master/_listings/predix/apiv1schedulerjobsid-put-openapi.md
- name: Analytics Runtime - Update an existing orchestration configuration entry.
  x-api-slug: apiv2configorchestrationsid-put
  description: Updates the orchestration configuration entry with given orchestration
    configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/existing/master/_listings/predix/apiv2configorchestrationsid-put-openapi.md
x-common:
- type: x-api-gallery
  url: http://predicthq.api.gallery.streamdata.io
- type: x-api-stack
  url: http://predix.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/predix
- type: x-documentation
  url: https://docs.predix.io/en-US/platform
- type: x-twitter
  url: https://twitter.com/Predix
- type: x-website
  url: https://www.predix.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---