---
name: Azure DevTest Labs
x-slug: azure-devtest-labs
description: Azure DevTest Labs makes it easy to quickly create environments to deploy
  and test applications. Use reusable templates and artifacts to build Windows and
  Linux environments while minimalizing waste and controlling costs.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-devtest-integrate.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Labs
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/labs/master/_listings/azure-devtest-labs/apis.md
specificationVersion: "0.14"
apis:
- name: DevTestLabsClient - Labs List By Subscription
  x-api-slug: subscriptionssubscriptionidprovidersmicrosoft-devtestlablabs-get
  description: List labs in a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-devtest-integrate.png
  humanURL: https://azure.microsoft.com/en-us/services/devtest-lab/
  baseURL: ://management.azure.com//
  tags: Testing, Microsoft, Orchestration, Stack Network, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labs/master/_listings/azure-devtest-labs/subscriptionssubscriptionidprovidersmicrosoft-devtestlablabs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labs/master/_listings/azure-devtest-labs/subscriptionssubscriptionidprovidersmicrosoft-devtestlablabs-get-openapi.md
- name: DevTestLabsClient - Labs List By Resource Group
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabs-get
  description: List labs in a resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-devtest-integrate.png
  humanURL: https://azure.microsoft.com/en-us/services/devtest-lab/
  baseURL: ://management.azure.com//
  tags: Testing, Microsoft, Orchestration, Stack Network, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labs/master/_listings/azure-devtest-labs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labs/master/_listings/azure-devtest-labs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabs-get-openapi.md
- name: DevTestLabsClient - Labs Get
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsname-get
  description: Get lab.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-devtest-integrate.png
  humanURL: https://azure.microsoft.com/en-us/services/devtest-lab/
  baseURL: ://management.azure.com//
  tags: Testing, Microsoft, Orchestration, Stack Network, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labs/master/_listings/azure-devtest-labs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labs/master/_listings/azure-devtest-labs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsname-get-openapi.md
- name: DevTestLabsClient - Labs Create Or Update
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsname-put
  description: Create or replace an existing lab. This operation can take a while
    to complete.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-devtest-integrate.png
  humanURL: https://azure.microsoft.com/en-us/services/devtest-lab/
  baseURL: ://management.azure.com//
  tags: Testing, Microsoft, Orchestration, Stack Network, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labs/master/_listings/azure-devtest-labs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsname-put-openapi.md
- name: DevTestLabsClient - Labs Delete
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsname-delete
  description: Delete lab. This operation can take a while to complete.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-devtest-integrate.png
  humanURL: https://azure.microsoft.com/en-us/services/devtest-lab/
  baseURL: ://management.azure.com//
  tags: Testing, Microsoft, Orchestration, Stack Network, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labs/master/_listings/azure-devtest-labs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsname-delete-openapi.md
- name: DevTestLabsClient - Labs Update
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsname-patch
  description: Modify properties of labs.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-devtest-integrate.png
  humanURL: https://azure.microsoft.com/en-us/services/devtest-lab/
  baseURL: ://management.azure.com//
  tags: Testing, Microsoft, Orchestration, Stack Network, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labs/master/_listings/azure-devtest-labs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsname-patch-openapi.md
- name: DevTestLabsClient - Labs Claim Any Vm
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsnameclaimanyvm-post
  description: Claim a random claimable virtual machine in the lab. This operation
    can take a while to complete.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-devtest-integrate.png
  humanURL: https://azure.microsoft.com/en-us/services/devtest-lab/
  baseURL: ://management.azure.com//
  tags: Testing, Microsoft, Orchestration, Stack Network, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labs/master/_listings/azure-devtest-labs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsnameclaimanyvm-post-openapi.md
- name: DevTestLabsClient - Labs Generate Upload Uri
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsnamegenerateuploaduri-post
  description: Generate a URI for uploading custom disk images to a Lab.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-devtest-integrate.png
  humanURL: https://azure.microsoft.com/en-us/services/devtest-lab/
  baseURL: ://management.azure.com//
  tags: Testing, Microsoft, Orchestration, Stack Network, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/labs/master/_listings/azure-devtest-labs/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsnamegenerateuploaduri-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://azure.data.lake.store.api.gallery.streamdata.io
- type: x-api-stack
  url: http://azure.devtest.labs.stack.network
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/devtest-lab/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/devtest-lab/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/devtest-lab/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/devtest-lab/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---