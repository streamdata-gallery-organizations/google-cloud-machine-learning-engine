---
swagger: "2.0"
x-collection-name: Google Cloud Machine Learning Engine
x-complete: 0
info:
  title: Google Cloud Machine Learning API Get Operations
  description: |-
    Lists operations that match the specified filter in the request. If the
    server doesn't support this method, it returns `UNIMPLEMENTED`.

    NOTE: the `name` binding below allows API services to override the binding
    to use different resource name schemes, such as `users/*/operations`.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: ml.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{name}:
    delete:
      summary: Delete Model Version
      description: |-
        Deletes a model version.

        Each model can have multiple versions deployed and in use at any given
        time. Use this method to remove a single version.

        Note: You cannot delete the version that is set as the default version
        of the model unless it is the only remaining version.
      operationId: ml.projects.models.versions.delete
      x-api-path-slug: v1name-delete
      parameters:
      - in: path
        name: name
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Version
    get:
      summary: Get Model Version
      description: |-
        Gets information about a model version.

        Models can have multiple versions. You can call
        [projects.models.versions.list](/ml/reference/rest/v1/projects.models.versions/list)
        to get the same information that this method returns for all of the
        versions of a model.
      operationId: ml.projects.models.versions.get
      x-api-path-slug: v1name-get
      parameters:
      - in: path
        name: name
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Version
  /v1/{name}/operations:
    get:
      summary: Get Operations
      description: |-
        Lists operations that match the specified filter in the request. If the
        server doesn't support this method, it returns `UNIMPLEMENTED`.

        NOTE: the `name` binding below allows API services to override the binding
        to use different resource name schemes, such as `users/*/operations`.
      operationId: ml.projects.operations.list
      x-api-path-slug: v1nameoperations-get
      parameters:
      - in: query
        name: filter
        description: The standard list filter
      - in: path
        name: name
        description: The name of the operation collection
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
      - Machine Learning
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