{
  "info": {
    "name": "Plivo SMS Send Message",
    "_postman_id": "f8b3f4a8-b2bd-4b61-9c52-00ad5244c70d",
    "description": "This API enables you to send messages via Plivou2019s SMS service.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Message",
      "item": [
        {
          "id": "f3369f2e-ef04-4876-b0d5-500aa53a4e72",
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
              "id": "6a402707-d5d9-4a52-b259-a30e95fe818d"
            }
          ]
        }
      ]
    },
    {
      "name": "Send",
      "item": [
        {
          "id": "189880a3-82c2-4b4e-acc5-8f3cfbf505ba",
          "name": "postAuthMessage",
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
                  "key": "dst",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "log",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "method",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "src",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "text",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "This API enables you to send messages via Plivou2019s SMS service.",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "auth_id",
                  "value": "auth_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "This API enables you to send messages via Plivou2019s SMS service."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c83dee91-e058-4049-9a3e-f731b2e98f1d"
            }
          ]
        }
      ]
    }
  ]
}