---
swagger: "2.0"
x-collection-name: Azure DevTest Labs
x-complete: 0
info:
  title: Azure DevTest Labs API Labs List Vhds
  description: List disk images available for custom image creation.
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
  /subscriptions/{subscriptionId}/providers/Microsoft.DevTestLab/labs:
    get:
      summary: Labs List By Subscription
      description: List labs in a subscription.
      operationId: Labs_ListBySubscription
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-devtestlablabs-get
      parameters:
      - in: query
        name: $expand
        description: Specify the $expand query
      - in: query
        name: $filter
        description: The filter to apply to the operation
      - in: query
        name: $orderby
        description: The ordering expression for the results, using OData notation
      - in: query
        name: $top
        description: The maximum number of resources to return from the operation
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Labs
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevTestLab/labs:
    get:
      summary: Labs List By Resource Group
      description: List labs in a resource group.
      operationId: Labs_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabs-get
      parameters:
      - in: query
        name: $expand
        description: Specify the $expand query
      - in: query
        name: $filter
        description: The filter to apply to the operation
      - in: query
        name: $orderby
        description: The ordering expression for the results, using OData notation
      - in: query
        name: $top
        description: The maximum number of resources to return from the operation
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Labs
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevTestLab/labs/{name}:
    get:
      summary: Labs Get
      description: Get lab.
      operationId: Labs_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsname-get
      parameters:
      - in: query
        name: $expand
        description: Specify the $expand query
      - in: path
        name: name
        description: The name of the lab
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Labs
    put:
      summary: Labs Create Or Update
      description: Create or replace an existing lab. This operation can take a while
        to complete.
      operationId: Labs_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsname-put
      parameters:
      - in: body
        name: lab
        description: A lab
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The name of the lab
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Labs
    delete:
      summary: Labs Delete
      description: Delete lab. This operation can take a while to complete.
      operationId: Labs_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsname-delete
      parameters:
      - in: path
        name: name
        description: The name of the lab
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Labs
    patch:
      summary: Labs Update
      description: Modify properties of labs.
      operationId: Labs_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsname-patch
      parameters:
      - in: body
        name: lab
        description: A lab
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The name of the lab
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Labs
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevTestLab/labs/{name}/claimAnyVm:
    post:
      summary: Labs Claim Any Vm
      description: Claim a random claimable virtual machine in the lab. This operation
        can take a while to complete.
      operationId: Labs_ClaimAnyVm
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsnameclaimanyvm-post
      parameters:
      - in: path
        name: name
        description: The name of the lab
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Labs
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevTestLab/labs/{name}/createEnvironment:
    post:
      summary: Labs Create Environment
      description: Create virtual machines in a lab. This operation can take a while
        to complete.
      operationId: Labs_CreateEnvironment
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsnamecreateenvironment-post
      parameters:
      - in: body
        name: labVirtualMachineCreationParameter
        description: Properties for creating a virtual machine
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The name of the lab
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Labs Environment
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevTestLab/labs/{name}/exportResourceUsage
  : post:
      summary: Labs Export Resource Usage
      description: Exports the lab resource usage into a storage account This operation
        can take a while to complete.
      operationId: Labs_ExportResourceUsage
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsnameexportresourceusage-post
      parameters:
      - in: body
        name: exportResourceUsageParameters
        description: The parameters of the export operation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The name of the lab
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Labs Export
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevTestLab/labs/{name}/generateUploadUri:
    post:
      summary: Labs Generate Upload Uri
      description: Generate a URI for uploading custom disk images to a Lab.
      operationId: Labs_GenerateUploadUri
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsnamegenerateuploaduri-post
      parameters:
      - in: body
        name: generateUploadUriParameter
        description: Properties for generating an upload URI
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The name of the lab
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Labs
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DevTestLab/labs/{name}/listVhds:
    post:
      summary: Labs List Vhds
      description: List disk images available for custom image creation.
      operationId: Labs_ListVhds
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-devtestlablabsnamelistvhds-post
      parameters:
      - in: path
        name: name
        description: The name of the lab
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Labs Vhds
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---