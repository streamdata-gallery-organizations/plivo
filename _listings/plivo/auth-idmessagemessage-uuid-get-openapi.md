---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 0
info:
  title: Plivo SMS Message
  version: v1
  description: Get details of a single message.
host: api.plivo.com
basePath: v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  '{auth_id}/Message/':
    get:
      summary: Message
      description: Get details of a message.
      operationId: getAuthMessage
      x-api-path-slug: auth-idmessage-get
      parameters:
      - in: path
        name: auth_id
        description: AUTH TOKEN Your Plivo AUTH ID and AUTH TOKEN can be found when
          you login to your dashboard
      - in: query
        name: limit
        description: Used to display the number of results per page
      - in: query
        name: offset
        description: Denotes the number of value items by which the results should
          be offset
      responses:
        200:
          description: OK
      tags:
      - Message
    post:
      summary: Send Message
      description: This API enables you to send messages via Plivou2019s SMS service.
      operationId: postAuthMessage
      x-api-path-slug: auth-idmessage-post
      parameters:
      - in: query
        name: dst
        description: The number to which the message needs to be sent
      - in: query
        name: log
        description: If set to false, the content of this message will not be logged
          on the Plivo infrastructure and the dst value will be masked
      - in: query
        name: method
        description: The method used to call the url
      - in: query
        name: src
        description: The phone number to be used as the caller id (with the country
          code)
      - in: query
        name: text
        description: The text to send encoded in Unicode UTF-8
      - in: path
        name: This API enables you to send messages via Plivou2019s SMS service.
        description: AUTH TOKEN Your Plivo AUTH ID and AUTH TOKEN can be found when
          you login to your dashboard
      - in: query
        name: type
        description: The type of message
      - in: query
        name: url
        description: The URL to which with the status of the message is sent
      responses:
        200:
          description: OK
      tags:
      - Send
      - Message
  '{auth_id}/Message/{message_uuid}/':
    get:
      summary: Message
      description: Get details of a single message.
      operationId: getAuthMessageMessageUu
      x-api-path-slug: auth-idmessagemessage-uuid-get
      parameters:
      - in: query
        name: auth_id
        description: AUTH TOKEN Your Plivo AUTH ID and AUTH TOKEN can be found when
          you login to your dashboard
      - in: path
        name: message_uuid
        description: The message unique id
      responses:
        200:
          description: OK
      tags:
      - Message
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---