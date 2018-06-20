---
name: Google Cloud Machine Learning Engine
x-slug: google-cloud-machine-learning-engine
description: Google Cloud Machine Learning Engine is a managed service that enables
  you to easily build machine learning models, that work on any type of data, of any
  size. Create your model with the powerful TensorFlow framework that powers many
  Google products, from Google Photos to Google Cloud Speech. Build models of any
  size with our managed scalable infrastructure. Your trained model is immediately
  available for use with our global prediction platform that can support thousands
  of users and TBs of data.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-ml.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Google Cloud Machine Learning Engine
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-machine-learning-engine/master/_listings/google-cloud-machine-learning-engine/apis.md
specificationVersion: "0.14"
apis:
- name: Google Cloud Machine Learning API Delete Model Version
  x-api-slug: google-cloud-machine-learning-api
  description: |-
    Deletes a model version.

    Each model can have multiple versions deployed and in use at any given
    time. Use this method to remove a single version.

    Note: You cannot delete the version that is set as the default version
    of the model unless it is the only remaining version.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-ml.png
  humanURL: https://cloud.google.com/ml-engine/
  baseURL: ://ml.googleapis.com////v1/{name}
  tags: Machine Learning,Version
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-machine-learning-engine/master/_listings/google-cloud-machine-learning-engine/v1name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-machine-learning-engine/master/_listings/google-cloud-machine-learning-engine/v1name-delete-openapi.md
- name: Google Cloud Machine Learning API Get Model Version
  x-api-slug: google-cloud-machine-learning-api
  description: |-
    Gets information about a model version.

    Models can have multiple versions. You can call
    [projects.models.versions.list](/ml/reference/rest/v1/projects.models.versions/list)
    to get the same information that this method returns for all of the
    versions of a model.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-ml.png
  humanURL: https://cloud.google.com/ml-engine/
  baseURL: ://ml.googleapis.com////v1/{name}
  tags: Machine Learning,Version
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-machine-learning-engine/master/_listings/google-cloud-machine-learning-engine/v1name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-machine-learning-engine/master/_listings/google-cloud-machine-learning-engine/v1name-get-openapi.md
- name: Google Cloud Machine Learning API Get Operations
  x-api-slug: google-cloud-machine-learning-api
  description: |-
    Lists operations that match the specified filter in the request. If the
    server doesn't support this method, it returns `UNIMPLEMENTED`.

    NOTE: the `name` binding below allows API services to override the binding
    to use different resource name schemes, such as `users/*/operations`.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-ml.png
  humanURL: https://cloud.google.com/ml-engine/
  baseURL: ://ml.googleapis.com////v1/{name}/operations
  tags: Machine Learning,Operation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-machine-learning-engine/master/_listings/google-cloud-machine-learning-engine/v1nameoperations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-machine-learning-engine/master/_listings/google-cloud-machine-learning-engine/v1nameoperations-get-openapi.md
- name: Google Cloud Machine Learning API Cancel Operation
  x-api-slug: google-cloud-machine-learning-api
  description: |-
    Starts asynchronous cancellation on a long-running operation.  The server
    makes a best effort to cancel the operation, but success is not
    guaranteed.  If the server doesn't support this method, it returns
    `google.rpc.Code.UNIMPLEMENTED`.  Clients can use
    Operations.GetOperation or
    other methods to check whether the cancellation succeeded or whether the
    operation completed despite cancellation. On successful cancellation,
    the operation is not deleted; instead, it becomes an operation with
    an Operation.error value with a google.rpc.Status.code of 1,
    corresponding to `Code.CANCELLED`.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-ml.png
  humanURL: https://cloud.google.com/ml-engine/
  baseURL: ://ml.googleapis.com////v1/{name}:cancel
  tags: Machine Learning,Operation
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-machine-learning-engine/master/_listings/google-cloud-machine-learning-engine/v1namecancel-post-openapi.md
- name: Google Cloud Machine Learning API Get Operation
  x-api-slug: google-cloud-machine-learning-api
  description: |-
    Get the service account information associated with your project. You need
    this information in order to grant the service account persmissions for
    the Google Cloud Storage location where you put your model training code
    for training the model with Google Cloud Machine Learning.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-ml.png
  humanURL: https://cloud.google.com/ml-engine/
  baseURL: ://ml.googleapis.com////v1/{name}:getConfig
  tags: Machine Learning,Operation
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-machine-learning-engine/master/_listings/google-cloud-machine-learning-engine/v1namegetconfig-get-openapi.md
- name: Google Cloud Machine Learning API Predict Operation
  x-api-slug: google-cloud-machine-learning-api
  description: |-
    Performs prediction on the data in the request.

    **** REMOVE FROM GENERATED DOCUMENTATION
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-ml.png
  humanURL: https://cloud.google.com/ml-engine/
  baseURL: ://ml.googleapis.com////v1/{name}:predict
  tags: Machine Learning,Operation
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-machine-learning-engine/master/_listings/google-cloud-machine-learning-engine/v1namepredict-post-openapi.md
- name: Google Cloud Machine Learning API Set Default Version
  x-api-slug: google-cloud-machine-learning-api
  description: |-
    Designates a version to be the default for the model.

    The default version is used for prediction requests made against the model
    that don't specify a version.

    The first version to be created for a model is automatically set as the
    default. You must make any subsequent changes to the default version
    setting manually using this method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-ml.png
  humanURL: https://cloud.google.com/ml-engine/
  baseURL: ://ml.googleapis.com////v1/{name}:setDefault
  tags: Machine Learning,Version
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-machine-learning-engine/master/_listings/google-cloud-machine-learning-engine/v1namesetdefault-post-openapi.md
- name: Google Cloud Machine Learning API List Jobs
  x-api-slug: google-cloud-machine-learning-api
  description: Lists the jobs in the project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-ml.png
  humanURL: https://cloud.google.com/ml-engine/
  baseURL: ://ml.googleapis.com////v1/{parent}/jobs
  tags: Machine Learning,Job
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-machine-learning-engine/master/_listings/google-cloud-machine-learning-engine/v1parentjobs-get-openapi.md
- name: Google Cloud Machine Learning API Create Job
  x-api-slug: google-cloud-machine-learning-api
  description: Creates a training or a batch prediction job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-ml.png
  humanURL: https://cloud.google.com/ml-engine/
  baseURL: ://ml.googleapis.com////v1/{parent}/jobs
  tags: Machine Learning,Job
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-machine-learning-engine/master/_listings/google-cloud-machine-learning-engine/v1parentjobs-post-openapi.md
- name: Google Cloud Machine Learning API List Models
  x-api-slug: google-cloud-machine-learning-api
  description: |-
    Lists the models in a project.

    Each project can contain multiple models, and each model can have multiple
    versions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-ml.png
  humanURL: https://cloud.google.com/ml-engine/
  baseURL: ://ml.googleapis.com////v1/{parent}/models
  tags: Machine Learning,Model
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-machine-learning-engine/master/_listings/google-cloud-machine-learning-engine/v1parentmodels-get-openapi.md
- name: Google Cloud Machine Learning API Create Models
  x-api-slug: google-cloud-machine-learning-api
  description: |-
    Creates a model which will later contain one or more versions.

    You must add at least one version before you can request predictions from
    the model. Add versions by calling
    [projects.models.versions.create](/ml/reference/rest/v1/projects.models.versions/create).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-ml.png
  humanURL: https://cloud.google.com/ml-engine/
  baseURL: ://ml.googleapis.com////v1/{parent}/models
  tags: Machine Learning,Model
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-machine-learning-engine/master/_listings/google-cloud-machine-learning-engine/v1parentmodels-post-openapi.md
- name: Google Cloud Machine Learning API Get Version
  x-api-slug: google-cloud-machine-learning-api
  description: |-
    Gets basic information about all the versions of a model.

    If you expect that a model has a lot of versions, or if you need to handle
    only a limited number of results at a time, you can request that the list
    be retrieved in batches (called pages):
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-ml.png
  humanURL: https://cloud.google.com/ml-engine/
  baseURL: ://ml.googleapis.com////v1/{parent}/versions
  tags: Machine Learning,Version
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-machine-learning-engine/master/_listings/google-cloud-machine-learning-engine/v1parentversions-get-openapi.md
- name: Google Cloud Machine Learning API Create Version
  x-api-slug: google-cloud-machine-learning-api
  description: |-
    Creates a new version of a model from a trained TensorFlow model.

    If the version created in the cloud by this call is the first deployed
    version of the specified model, it will be made the default version of the
    model. When you add a version to a model that already has one or more
    versions, the default version does not automatically change. If you want a
    new version to be the default, you must call
    [projects.models.versions.setDefault](/ml/reference/rest/v1/projects.models.versions/setDefault).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-ml.png
  humanURL: https://cloud.google.com/ml-engine/
  baseURL: ://ml.googleapis.com////v1/{parent}/versions
  tags: Machine Learning,Version
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-machine-learning-engine/master/_listings/google-cloud-machine-learning-engine/v1parentversions-post-openapi.md
- name: Google Cloud Machine Learning API
  x-api-slug: google-cloud-machine-learning-api
  description: Google Cloud Machine Learning Engine is a managed service that enables
    you to easily build machine learning models, that work on any type of data, of
    any size. Create your model with the powerful TensorFlow framework that powers
    many Google products, from Google Photos to Google Cloud Speech. Build models
    of any size with our managed scalable infrastructure. Your trained model is immediately
    available for use with our global prediction platform that can support thousands
    of users and TBs of data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-ml.png
  humanURL: https://cloud.google.com/ml-engine/
  baseURL: ://ml.googleapis.com//
  tags: Google Cloud Machine Learning Engine
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-machine-learning-engine/master/_listings/google-cloud-machine-learning-engine/openapi.md
x-common:
- type: x-change-log
  url: https://cloud.google.com/ml-engine/docs/resources/release-notes
- type: x-command-line-interface
  url: https://cloud.google.com/sdk/gcloud/reference/ml-engine/
- type: x-concepts
  url: https://cloud.google.com/ml-engine/docs/concepts/
- type: x-documentation
  url: https://cloud.google.com/ml-engine/docs/
- type: x-getting-started
  url: https://cloud.google.com/ml-engine/docs/quickstarts/
- type: x-pricing
  url: https://cloud.google.com/ml-engine/pricing
- type: x-rate-limits
  url: https://cloud.google.com/ml-engine/quotas
- type: x-service-level-agreements
  url: https://cloud.google.com/ml-engine/sla
- type: x-support
  url: https://cloud.google.com/ml-engine/docs/resources/support
- type: x-terms-of-service
  url: https://cloud.google.com/terms/
- type: x-tutorials
  url: https://cloud.google.com/ml-engine/docs/tutorials/
- type: x-versioning
  url: https://cloud.google.com/ml-engine/docs/concepts/versioning
- type: x-website
  url: https://cloud.google.com/ml-engine/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---