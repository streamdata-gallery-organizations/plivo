---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 0
info:
  title: Codenvy Account API Get Account Members
  description: Get all members for a specific account. This API call requires account/owner,
    system/admin or system/manager role.
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
  /account/subscriptions/{subscriptionId}:
    delete:
      summary: Delete Account Subscriptions Subscriptionid
      description: 'Remove subscription from account. Roles: account/owner, system/admin.'
      operationId: removeSubscription
      x-api-path-slug: accountsubscriptionssubscriptionid-delete
      parameters:
      - in: path
        name: subscriptionId
        description: Subscription ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Subscriptions
      - SubscriptionId
    get:
      summary: Get Account Subscriptions Subscriptionid
      description: Get information on a particular subscription by its unique ID.
      operationId: getSubscriptionById
      x-api-path-slug: accountsubscriptionssubscriptionid-get
      parameters:
      - in: path
        name: subscriptionId
        description: Subscription ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Subscriptions
      - SubscriptionId
  /account/{accountId}/subscriptions:
    get:
      summary: Get Account Accountid Subscriptions
      description: Get information on account subscriptions. This API call requires
        account/owner, account/member, system/admin or system/manager role.
      operationId: getSubscriptions
      x-api-path-slug: accountaccountidsubscriptions-get
      parameters:
      - in: path
        name: accountId
        description: Account ID
      - in: query
        name: service
        description: Service ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - AccountId
      - Subscriptions
  /account/{id}:
    delete:
      summary: Delete Account
      description: Remove subscription from account. JSON with subscription details
        is sent. Can be performed only by system/admin.
      operationId: remove
      x-api-path-slug: accountid-delete
      parameters:
      - in: path
        name: id
        description: Account ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
    get:
      summary: Get Account
      description: Get account information by its ID. JSON with account details is
        returned. This API call requires account/owner, system/admin or system/manager
        role.
      operationId: getById
      x-api-path-slug: accountid-get
      parameters:
      - in: path
        name: id
        description: Account ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
    post:
      summary: Post Account
      description: Update account. This API call requires account/owner role.
      operationId: update
      x-api-path-slug: accountid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Account ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
  /account/{id}/attribute:
    delete:
      summary: Delete Account Attribute
      description: Remove attribute from an account. Attribute name is used as a quary
        parameter. For this API request account/owner, system/admin or system/manager
        role is required
      operationId: removeAttribute
      x-api-path-slug: accountidattribute-delete
      parameters:
      - in: path
        name: id
        description: Account ID
      - in: query
        name: name
        description: Attribute name to be removed
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
      - Attribute
  /account/{id}/members:
    get:
      summary: Get Account Members
      description: Get all members for a specific account. This API call requires
        account/owner, system/admin or system/manager role.
      operationId: getMembers
      x-api-path-slug: accountidmembers-get
      parameters:
      - in: path
        name: id
        description: Account ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
      - Members
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