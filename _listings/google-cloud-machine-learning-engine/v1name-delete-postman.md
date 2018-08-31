{
  "info": {
    "name": "Google Cloud Machine Learning API Delete Model Version",
    "_postman_id": "95433a7e-e89a-4e81-bd98-13a5e4c3f55b",
    "description": "Deletes a model version.\n\nEach model can have multiple versions deployed and in use at any given\ntime. Use this method to remove a single version.\n\nNote: You cannot delete the version that is set as the default version\nof the model unless it is the only remaining version.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Version",
      "item": [
        {
          "id": "86f28a1b-4994-4213-b9dd-2cbb0b11ebb0",
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
              "id": "0730fbf1-1347-4792-8682-ed05e25bee0e"
            }
          ]
        }
      ]
    }
  ]
}