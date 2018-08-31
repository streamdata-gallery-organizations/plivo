---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 0
info:
  title: Codenvy Account API Post Account Subscriptions
  description: 'Add a new subscription to an account. JSON with subscription details
    is sent. Roles: account/owner, system/admin.'
  version: 1.0.0
host: /account
basePath: https://codenvy.com/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account:
    get:
      summary: Get Account
      description: This API call returns a JSON with all user membership in a single
        or multiple accounts
      operationId: getMemberships
      x-api-path-slug: account-get
      responses:
        200:
          description: OK
      tags:
      - Account
    post:
      summary: Post Account
      description: Create a new account
      operationId: create
      x-api-path-slug: account-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
  /account/find:
    get:
      summary: Get Account Find
      description: Get account information by its name. JSON with account details
        is returned. This API call requires system/admin or system/manager role.
      operationId: getByName
      x-api-path-slug: accountfind-get
      parameters:
      - in: query
        name: name
        description: Account name
      responses:
        200:
          description: OK
      tags:
      - Account
      - Find
  /account/memberships:
    get:
      summary: Get Account Memberships
      description: ID of a user should be specified as a query parameter. JSON with
        membership details is returned. For this API call system/admin or system/manager
        role is required
      operationId: getMembershipsOfSpecificUser
      x-api-path-slug: accountmemberships-get
      parameters:
      - in: query
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Memberships
  /account/subscriptions:
    post:
      summary: Post Account Subscriptions
      description: 'Add a new subscription to an account. JSON with subscription details
        is sent. Roles: account/owner, system/admin.'
      operationId: addSubscription
      x-api-path-slug: accountsubscriptions-post
      parameters:
      - in: body
        name: body
        description: Subscription details
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Subscriptions
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