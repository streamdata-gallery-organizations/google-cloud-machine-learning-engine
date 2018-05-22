{
  "info": {
    "name": "Google Cloud Machine Learning API Get Operations",
    "_postman_id": "d0f42e73-cf24-4eb6-a845-4b713aac4540",
    "description": "Lists operations that match the specified filter in the request. If the\nserver doesn't support this method, it returns `UNIMPLEMENTED`.\n\nNOTE: the `name` binding below allows API services to override the binding\nto use different resource name schemes, such as `users/*/operations`.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Version",
      "item": [
        {
          "id": "c07b0ffa-4347-4fec-8156-5c3362513317",
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
              "id": "16f943bb-dbde-488e-9a83-8a1a48f4b3ab"
            }
          ]
        },
        {
          "id": "2db34e30-79da-40a2-98ef-4e5f1bc99610",
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
              "id": "a9334c03-adeb-409b-bca3-6f274f838ff1"
            }
          ]
        }
      ]
    },
    {
      "name": "Operation",
      "item": [
        {
          "id": "b297af89-acef-43b1-8287-077b787a199b",
          "name": "ml.projects.operations.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "ml.googleapis.com",
              "path": [
                "v1/:name/operations"
              ],
              "query": [
                {
                  "key": "filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageSize",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Lists operations that match the specified filter in the request. If the\nserver doesn't support this method, it returns `UNIMPLEMENTED`.\n\nNOTE: the `name` binding below allows API services to override the binding\nto use different resource name schemes, such as `users/*/operations`."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47b64f8f-62c7-40dc-9174-c493c5c8c4a0"
            }
          ]
        }
      ]
    }
  ]
}