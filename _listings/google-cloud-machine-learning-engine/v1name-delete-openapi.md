---
swagger: "2.0"
x-collection-name: Google Cloud Machine Learning Engine
x-complete: 0
info:
  title: Google Cloud Machine Learning API Delete Model Version
  description: |-
    Deletes a model version.

    Each model can have multiple versions deployed and in use at any given
    time. Use this method to remove a single version.

    Note: You cannot delete the version that is set as the default version
    of the model unless it is the only remaining version.
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