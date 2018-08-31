---
swagger: "2.0"
info:
  title: Google Cloud Machine Learning Engine
  description: An API to enable creating and using machine learning models.
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
  /v1/{parent}/jobs:
    get:
      summary: List Jobs
      description: Lists the jobs in the project
      operationId: ml.projects.jobs.list
      parameters:
      - in: query
        name: filter
        description: Optional
      - in: query
        name: pageSize
        description: Optional
      - in: query
        name: pageToken
        description: Optional
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - job
definitions:
  GoogleApi__HttpBody:
    properties:
      contentType:
        description: This is a default description.
        type: post
      data:
        description: This is a default description.
        type: post
  GoogleCloudMlV1_HyperparameterOutput_HyperparameterMetric:
    properties:
      objectiveValue:
        description: This is a default description.
        type: post
      trainingStep:
        description: This is a default description.
        type: post
  GoogleCloudMlV1__CancelJobRequest:
    properties: []
  GoogleCloudMlV1__GetConfigResponse:
    properties:
      serviceAccount:
        description: This is a default description.
        type: post
      serviceAccountProject:
        description: This is a default description.
        type: post
  GoogleCloudMlV1__HyperparameterOutput:
    properties:
      allMetrics:
        description: This is a default description.
        type: post
      hyperparameters:
        description: This is a default description.
        type: post
      trialId:
        description: This is a default description.
        type: post
  GoogleCloudMlV1__HyperparameterSpec:
    properties:
      goal:
        description: This is a default description.
        type: post
      hyperparameterMetricTag:
        description: This is a default description.
        type: post
      maxParallelTrials:
        description: This is a default description.
        type: post
      maxTrials:
        description: This is a default description.
        type: post
      params:
        description: This is a default description.
        type: post
  GoogleCloudMlV1__Job:
    properties:
      createTime:
        description: This is a default description.
        type: post
      endTime:
        description: This is a default description.
        type: post
      errorMessage:
        description: This is a default description.
        type: post
      jobId:
        description: This is a default description.
        type: post
      startTime:
        description: This is a default description.
        type: post
      state:
        description: This is a default description.
        type: post
  GoogleCloudMlV1__ListJobsResponse:
    properties:
      jobs:
        description: This is a default description.
        type: post
      nextPageToken:
        description: This is a default description.
        type: post
  GoogleCloudMlV1__ListModelsResponse:
    properties:
      models:
        description: This is a default description.
        type: post
      nextPageToken:
        description: This is a default description.
        type: post
  GoogleCloudMlV1__ListVersionsResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: post
      versions:
        description: This is a default description.
        type: post
  GoogleCloudMlV1__ManualScaling:
    properties:
      nodes:
        description: This is a default description.
        type: post
  GoogleCloudMlV1__Model:
    properties:
      description:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      onlinePredictionLogging:
        description: This is a default description.
        type: post
      regions:
        description: This is a default description.
        type: post
  GoogleCloudMlV1__OperationMetadata:
    properties:
      createTime:
        description: This is a default description.
        type: post
      endTime:
        description: This is a default description.
        type: post
      isCancellationRequested:
        description: This is a default description.
        type: post
      modelName:
        description: This is a default description.
        type: post
      operationType:
        description: This is a default description.
        type: post
      startTime:
        description: This is a default description.
        type: post
  GoogleCloudMlV1__ParameterSpec:
    properties:
      categoricalValues:
        description: This is a default description.
        type: post
      discreteValues:
        description: This is a default description.
        type: post
      maxValue:
        description: This is a default description.
        type: post
      minValue:
        description: This is a default description.
        type: post
      parameterName:
        description: This is a default description.
        type: post
      scaleType:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
  GoogleCloudMlV1__PredictRequest:
    properties: []
  GoogleCloudMlV1__PredictionInput:
    properties:
      dataFormat:
        description: This is a default description.
        type: post
      inputPaths:
        description: This is a default description.
        type: post
      maxWorkerCount:
        description: This is a default description.
        type: post
      modelName:
        description: This is a default description.
        type: post
      outputPath:
        description: This is a default description.
        type: post
      region:
        description: This is a default description.
        type: post
      runtimeVersion:
        description: This is a default description.
        type: post
      uri:
        description: This is a default description.
        type: post
      versionName:
        description: This is a default description.
        type: post
  GoogleCloudMlV1__PredictionOutput:
    properties:
      errorCount:
        description: This is a default description.
        type: post
      nodeHours:
        description: This is a default description.
        type: post
      outputPath:
        description: This is a default description.
        type: post
      predictionCount:
        description: This is a default description.
        type: post
  GoogleCloudMlV1__SetDefaultVersionRequest:
    properties: []
  GoogleCloudMlV1__TrainingInput:
    properties:
      args:
        description: This is a default description.
        type: post
      jobDir:
        description: This is a default description.
        type: post
      masterType:
        description: This is a default description.
        type: post
      packageUris:
        description: This is a default description.
        type: post
      parameterServerCount:
        description: This is a default description.
        type: post
      parameterServerType:
        description: This is a default description.
        type: post
      pythonModule:
        description: This is a default description.
        type: post
      region:
        description: This is a default description.
        type: post
      runtimeVersion:
        description: This is a default description.
        type: post
      scaleTier:
        description: This is a default description.
        type: post
  GoogleCloudMlV1__TrainingOutput:
    properties:
      completedTrialCount:
        description: This is a default description.
        type: post
      consumedMLUnits:
        description: This is a default description.
        type: post
      isHyperparameterTuningJob:
        description: This is a default description.
        type: post
      trials:
        description: This is a default description.
        type: post
  GoogleCloudMlV1__Version:
    properties:
      createTime:
        description: This is a default description.
        type: post
      deploymentUri:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      isDefault:
        description: This is a default description.
        type: post
      lastUseTime:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      runtimeVersion:
        description: This is a default description.
        type: post
  GoogleCloudMlV1beta1__ManualScaling:
    properties:
      nodes:
        description: This is a default description.
        type: post
  GoogleCloudMlV1beta1__OperationMetadata:
    properties:
      createTime:
        description: This is a default description.
        type: post
      endTime:
        description: This is a default description.
        type: post
      isCancellationRequested:
        description: This is a default description.
        type: post
      modelName:
        description: This is a default description.
        type: post
      operationType:
        description: This is a default description.
        type: post
      startTime:
        description: This is a default description.
        type: post
  GoogleCloudMlV1beta1__Version:
    properties:
      createTime:
        description: This is a default description.
        type: post
      deploymentUri:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      isDefault:
        description: This is a default description.
        type: post
      lastUseTime:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      runtimeVersion:
        description: This is a default description.
        type: post
  GoogleLongrunning__ListOperationsResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: post
      operations:
        description: This is a default description.
        type: post
  GoogleLongrunning__Operation:
    properties:
      done:
        description: This is a default description.
        type: post
      metadata:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      response:
        description: This is a default description.
        type: post
  GoogleProtobuf__Empty:
    properties: []
  GoogleRpc__Status:
    properties:
      code:
        description: This is a default description.
        type: post
      details:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
x-collection-name: Google Cloud Machine Learning Engine
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