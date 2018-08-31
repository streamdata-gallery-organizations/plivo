{
  "info": {
    "name": "Codenvy Account API Post Comments Comments",
    "_postman_id": "fb2e1e68-e7a1-4d52-9acf-9e36a19426cc",
    "description": "Creates a reply to an existing comment. Comments can only be nested one level deep, you cannot reply to a reply of a comment. If a comment has a non-null parent_id value then it cannot be replied to.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blogs",
      "item": [
        {
          "id": "ed9bc326-83f7-4296-8f70-28bb33f491a7",
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
              "id": "011bf0d1-6890-4fb9-ba0b-5d0fa2a7fecc"
            }
          ]
        }
      ]
    },
    {
      "name": "Comments",
      "item": [
        {
          "id": "14cf0ce2-be72-42cd-b7ed-75f86fb061fe",
          "name": "creates-a-reply-to-an-existing-comment-comments-can-only-be-nested-one-level-deep-you-cannot-reply-t",
          "request": {
            "url": "http:///account/https://codenvy.com/api/comments/:id/comments?body (required)=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a reply to an existing comment. Comments can only be nested one level deep, you cannot reply to a reply of a comment. If a comment has a non-null parent_id value then it cannot be replied to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8175d01c-b4a4-4251-b78d-b0b841fea1ce"
            }
          ]
        }
      ]
    }
  ]
}