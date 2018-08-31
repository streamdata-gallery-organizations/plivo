{
  "info": {
    "name": "Codenvy Account API Put Blogs",
    "_postman_id": "d9da8ded-e0af-4eef-8263-a32786df59c4",
    "description": "Updates the Story.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blogs",
      "item": [
        {
          "id": "01df860a-3a09-4551-8060-004433404b33",
          "name": "creates-a-new-story",
          "request": {
            "url": "http:///account/https://codenvy.com/api/blogs/?body (required)=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&photo_ids=%7B%7D&tags=%7B%7D&title (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Story."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "afc08823-5512-4bcc-ab66-949d47a0d5d2"
            }
          ]
        },
        {
          "id": "b09d291b-7fa7-4983-bdb2-e501ee2f34b8",
          "name": "updates-the-story",
          "request": {
            "url": "http:///account/https://codenvy.com/api/blogs/:id?body=%7B%7D&id (required)=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&photo_ids=%7B%7D&tags=%7B%7D&title=%7B%7D",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the Story."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a1f3f3b-2fa4-40c0-9006-2a058e4afbd2"
            }
          ]
        }
      ]
    }
  ]
}