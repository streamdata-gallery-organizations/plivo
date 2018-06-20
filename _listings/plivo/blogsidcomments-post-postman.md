{
  "info": {
    "name": "Codenvy Account API Post Blogs Comments",
    "_postman_id": "02a14379-a355-4748-83a6-8b86a71eeb51",
    "description": "Creates a comment for the Story.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blogs",
      "item": [
        {
          "id": "0b4cd1bc-0c68-485e-b224-bb11adb77b52",
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
              "id": "2b938974-a6e6-4316-8b7f-20b8d3295a3a"
            }
          ]
        },
        {
          "id": "c6258466-d27d-4838-b688-6e36aa9f3a34",
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
              "id": "cd6851f1-0a2e-4b4d-a1e7-25de44e35a9e"
            }
          ]
        },
        {
          "id": "10e58c5e-768f-4c0d-b437-1f97758157db",
          "name": "creates-a-comment-for-the-story",
          "request": {
            "url": "http:///account/https://codenvy.com/api/blogs/:id/comments?body (required)=%7B%7D&id (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a comment for the Story."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f2d58a7-99e4-4a3d-8e44-0773470e002c"
            }
          ]
        }
      ]
    }
  ]
}