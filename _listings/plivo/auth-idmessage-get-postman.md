{
  "info": {
    "name": "Plivo SMS Message",
    "_postman_id": "d2ce9a08-8a4b-45f5-9fdb-3f17a22ae9e6",
    "description": "Get details of a message.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Message",
      "item": [
        {
          "id": "ae21dd94-69b6-4000-a6ef-483042cd52de",
          "name": "getAuthMessage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.plivo.com",
              "path": [
                "v1",
                ":auth_id/Message/"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "auth_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get details of a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf59a985-3b75-4621-a9fb-89ce3b22baa8"
            }
          ]
        }
      ]
    }
  ]
}