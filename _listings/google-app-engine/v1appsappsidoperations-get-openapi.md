---
swagger: "2.0"
x-collection-name: Google App Engine
x-complete: 0
info:
  title: Google App Engine Admin API Get Operations
  description: 'Lists operations that match the specified filter in the request. If
    the server doesn''t support this method, it returns UNIMPLEMENTED.NOTE: the name
    binding below allows API services to override the binding to use different resource
    name schemes, such as users/*/operations.'
  contact:
    name: Google
    url: https://google.com
  version: v1
host: appengine.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/apps/{appsId}/operations:
    get:
      summary: Get Operations
      description: 'Lists operations that match the specified filter in the request.
        If the server doesn''t support this method, it returns UNIMPLEMENTED.NOTE:
        the name binding below allows API services to override the binding to use
        different resource name schemes, such as users/*/operations.'
      operationId: appengine.apps.operations.list
      x-api-path-slug: v1appsappsidoperations-get
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: query
        name: filter
        description: The standard list filter
      - in: query
        name: pageSize
        description: The standard list page size
      - in: query
        name: pageToken
        description: The standard list page token
      responses:
        200:
          description: OK
      tags:
      - Operation
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