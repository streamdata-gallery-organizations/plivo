{
  "info": {
    "name": "Codenvy Account API Get Account",
    "_postman_id": "b991c5f1-1a33-4a8c-97de-7ae44245d853",
    "description": "This API call returns a JSON with all user membership in a single or multiple accounts",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "7b3baf4a-4581-40e0-ad8a-b58eb944c273",
          "name": "getMemberships",
          "request": {
            "url": "http:///account/https://codenvy.com/api/account",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API call returns a JSON with all user membership in a single or multiple accounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "277093c6-f8d6-4073-bccd-d94aac1f4b3e"
            }
          ]
        }
      ]
    }
  ]
}