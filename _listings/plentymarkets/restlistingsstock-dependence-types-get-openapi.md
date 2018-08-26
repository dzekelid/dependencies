---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List listing stock dependence types
  description: Lists listing stock dependence types.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/listings/stock_dependence_types:
    get:
      summary: List listing stock dependence types
      description: Lists listing stock dependence types.
      operationId: getRestListingsStockDependenceTypes
      x-api-path-slug: restlistingsstock-dependence-types-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Stock
      - Dependence
      - Types
  /rest/listings/stock_dependence_types/{id}:
    get:
      summary: Get a listing stock dependence type
      description: Gets a listing stock dependence type by given ID.
      operationId: getRestListingsStockDependenceTypes
      x-api-path-slug: restlistingsstock-dependence-typesid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Stock
      - Dependence
      - Type
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