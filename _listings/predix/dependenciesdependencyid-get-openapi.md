---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Insights Get Dependencies Dependencyid
  description: Get dependencies dependencyid.
  termsOfService: urn:tos
  version: 1.0.0
host: insights-api.data-services.predix.io
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /dependencies:
    get:
      summary: Get Dependencies
      description: Get dependencies.
      operationId: getDependencyListUsingGET
      x-api-path-slug: dependencies-get
      parameters:
      - in: query
        name: page
        description: Results page you want to retrieve (0
      - in: query
        name: size
        description: Number of records per page
      - in: query
        name: sort
        description: 'Sorting criteria in the format: property(,asc|desc)'
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
    post:
      summary: Post Dependencies
      description: Post dependencies.
      operationId: createDependencyUsingPOST
      x-api-path-slug: dependencies-post
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
  /dependencies/deploy:
    post:
      summary: Post Dependencies Deploy
      description: Post dependencies deploy.
      operationId: deployDependencyUsingPOST_1
      x-api-path-slug: dependenciesdeploy-post
      parameters:
      - in: query
        name: id
        description: id
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
      - Deploy
  /dependencies/deploy/{dependencyId}:
    post:
      summary: Post Dependencies Deploy Dependencyid
      description: Post dependencies deploy dependencyid.
      operationId: deployDependencyUsingPOST
      x-api-path-slug: dependenciesdeploydependencyid-post
      parameters:
      - in: path
        name: dependencyId
        description: dependencyId
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
      - Deploy
      - Dependencyid
  /dependencies/tags:
    get:
      summary: Get Dependencies Tags
      description: Get dependencies tags.
      operationId: getAllDependencyTagsUsingGET
      x-api-path-slug: dependenciestags-get
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
      - Tags
  /dependencies/undeploy:
    post:
      summary: Post Dependencies Undeploy
      description: Post dependencies undeploy.
      operationId: undeployDependencyUsingPOST_1
      x-api-path-slug: dependenciesundeploy-post
      parameters:
      - in: query
        name: id
        description: id
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
      - Undeploy
  /dependencies/undeploy/{dependencyId}:
    post:
      summary: Post Dependencies Undeploy Dependencyid
      description: Post dependencies undeploy dependencyid.
      operationId: undeployDependencyUsingPOST
      x-api-path-slug: dependenciesundeploydependencyid-post
      parameters:
      - in: path
        name: dependencyId
        description: dependencyId
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
      - Undeploy
      - Dependencyid
  /dependencies/{dependencyId}:
    get:
      summary: Get Dependencies Dependencyid
      description: Get dependencies dependencyid.
      operationId: getDependencyUsingGET
      x-api-path-slug: dependenciesdependencyid-get
      parameters:
      - in: path
        name: dependencyId
        description: dependencyId
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
      - Dependencyid
    post:
      summary: Post Dependencies Dependencyid
      description: Post dependencies dependencyid.
      operationId: updateDependencyUsingPOST
      x-api-path-slug: dependenciesdependencyid-post
      parameters:
      - in: path
        name: dependencyId
        description: dependencyId
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
      - Dependencyid
    delete:
      summary: Delete Dependencies Dependencyid
      description: Delete dependencies dependencyid.
      operationId: deleteDependencyUsingDELETE
      x-api-path-slug: dependenciesdependencyid-delete
      parameters:
      - in: path
        name: dependencyId
        description: dependencyId
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
      - Dependencyid
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