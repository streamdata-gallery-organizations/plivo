---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 0
info:
  title: Plivo SMS Message
  version: v1
  description: Get details of a message.
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