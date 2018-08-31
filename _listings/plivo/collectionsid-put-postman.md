{
  "info": {
    "name": "Codenvy Account API Put Collections",
    "_postman_id": "fe6cd4f1-5001-4686-b123-211ef64b67cc",
    "description": "Updates collection.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Collections",
      "item": [
        {
          "id": "1e656bc5-5abd-41ee-9932-d46b569675d2",
          "name": "creates-new-a-collection",
          "request": {
            "url": "http:///account/https://codenvy.com/api/collections?kind=%7B%7D&path (required)=%7B%7D&photo_ids=%7B%7D&position=%7B%7D&title (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates new a collection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1efb93fb-28f4-436f-8aee-fc26b1e2cc84"
            }
          ]
        },
        {
          "id": "0226ea43-232e-4f6f-9ec3-993274539fbb",
          "name": "updates-collection",
          "request": {
            "url": "http:///account/https://codenvy.com/api/collections/:id?id (required)=%7B%7D&kind=%7B%7D&path=%7B%7D&photo_ids=%7B%7D&position=%7B%7D&title=%7B%7D",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates collection."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8731e04-8a47-4668-a3f5-599b23fe2abc"
            }
          ]
        }
      ]
    }
  ]
}