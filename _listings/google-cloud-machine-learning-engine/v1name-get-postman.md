{
  "info": {
    "name": "Google Cloud Machine Learning API Get Model Version",
    "_postman_id": "f401692b-fc8b-447a-82df-2c835541617f",
    "description": "Gets information about a model version.\n\nModels can have multiple versions. You can call\n[projects.models.versions.list](/ml/reference/rest/v1/projects.models.versions/list)\nto get the same information that this method returns for all of the\nversions of a model.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Version",
      "item": [
        {
          "id": "ad35abb9-71f5-4fd4-8ada-5eac0dfc3691",
          "name": "ml.projects.models.versions.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "ml.googleapis.com",
              "path": [
                "v1/:name"
              ],
              "variable": [
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a model version.\n\nModels can have multiple versions. You can call\n[projects.models.versions.list](/ml/reference/rest/v1/projects.models.versions/list)\nto get the same information that this method returns for all of the\nversions of a model."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cab376c7-b063-45cc-81af-d1ee7cdec282"
            }
          ]
        },
        {
          "id": "675f9555-0490-4519-bc47-62922b796db7",
          "name": "ml.projects.models.versions.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "ml.googleapis.com",
              "path": [
                "v1/:name"
              ],
              "variable": [
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a model version.\n\nEach model can have multiple versions deployed and in use at any given\ntime. Use this method to remove a single version.\n\nNote: You cannot delete the version that is set as the default version\nof the model unless it is the only remaining version."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d7f62fdd-ea92-4a2c-90d9-086d344bec7d"
            }
          ]
        }
      ]
    }
  ]
}