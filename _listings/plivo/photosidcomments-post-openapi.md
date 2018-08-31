---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 0
info:
  title: Codenvy Account API Post Photos Comments
  description: Creates a new comment for the photo.
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
    post:
      summary: Post Account Members
      description: Add a new user to an account. This user will have account/member
        role. This API call requires account/owner, system/admin or system/manager
        role.
      operationId: addMember
      x-api-path-slug: accountidmembers-post
      parameters:
      - in: body
        name: body
        description: New membership
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
      - Members
  /account/{id}/members/{userid}:
    delete:
      summary: Delete Account Members User
      description: Remove user from a specific account. This API call requires account/owner,
        system/admin or system/manager role.
      operationId: removeMember
      x-api-path-slug: accountidmembersuserid-delete
      parameters:
      - in: path
        name: id
        description: Account ID
      - in: path
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
      - Members
      - Userid
  /account/{id}/resources:
    get:
      summary: Get Account Resources
      description: 'Returns used resources, provided by subscriptions. Roles: account/owner,
        account/member, system/manager, system/admin.'
      operationId: getResources
      x-api-path-slug: accountidresources-get
      parameters:
      - in: path
        name: id
        description: Account ID
      - in: query
        name: serviceId
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
      - Resources
    post:
      summary: Post Account Resources
      description: 'Redistributes resources between workspaces. Roles: account/owner,
        system/manager, system/admin.'
      operationId: redistributeResources
      x-api-path-slug: accountidresources-post
      parameters:
      - in: body
        name: body
        description: Resources description
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
      - Resources
  /blogs/:
    post:
      summary: Post Blogs
      description: Creates a new Story.
      operationId: creates-a-new-story
      x-api-path-slug: blogs-post
      parameters:
      - in: query
        name: body (required)
        description: Content of the blog post
      - in: query
        name: latitude
        description: Latitude for the blog post
      - in: query
        name: longitude
        description: Longitude for the blog post
      - in: query
        name: photo_ids
        description: Comma separated list of Photo ID values to post with the blog
      - in: query
        name: tags
        description: Comma separated list of tags
      - in: query
        name: title (required)
        description: Title for the blog post
      responses:
        200:
          description: OK
      tags:
      - Blogs
  /blogs/:id:
    put:
      summary: Put Blogs
      description: Updates the Story.
      operationId: updates-the-story
      x-api-path-slug: blogsid-put
      parameters:
      - in: query
        name: body
        description: Content of the blog post
      - in: query
        name: id (required)
        description: The Blog Post ID to update
      - in: query
        name: latitude
        description: Latitude for the blog post
      - in: query
        name: longitude
        description: Longitude for the blog post
      - in: query
        name: photo_ids
        description: Comma separated list of Photo IDs for photos that are in the
          blog post
      - in: query
        name: tags
        description: Comma separated list of tags
      - in: query
        name: title
        description: Title for the blog post
      responses:
        200:
          description: OK
      tags:
      - Blogs
      - :id
  /blogs/:id/comments:
    post:
      summary: Post Blogs Comments
      description: Creates a comment for the Story.
      operationId: creates-a-comment-for-the-story
      x-api-path-slug: blogsidcomments-post
      parameters:
      - in: query
        name: body (required)
        description: Content of the comment
      - in: query
        name: id (required)
        description: The Story ID to create a comment for
      responses:
        200:
          description: OK
      tags:
      - Blogs
      - :id
      - Comments
  /collections:
    post:
      summary: Post Collections
      description: Creates new a collection.
      operationId: creates-new-a-collection
      x-api-path-slug: collections-post
      parameters:
      - in: query
        name: kind
        description: 'Kind of the Collection to be created Recognized values: 1 -
          Portfolio Set (default), 2 - Profile Set'
      - in: query
        name: path (required)
        description: Path where the collection will be accessible at 500px
      - in: query
        name: photo_ids
        description: Comma separated list of Photo ID values to post with the blog
      - in: query
        name: position
        description: Position of the collection in the list of collections
      - in: query
        name: title (required)
        description: Title for the collection
      responses:
        200:
          description: OK
      tags:
      - Collections
  /collections/:id:
    put:
      summary: Put Collections
      description: Updates collection.
      operationId: updates-collection
      x-api-path-slug: collectionsid-put
      parameters:
      - in: query
        name: id (required)
        description: Collection ID
      - in: query
        name: kind
        description: Change kind of the Collection
      - in: query
        name: path
        description: Path where the collection will be accessible at 500px
      - in: query
        name: photo_ids
        description: Comma separated list of Photo ID values that are in this collection
      - in: query
        name: position
        description: Position of the collection in the list of collections
      - in: query
        name: title
        description: Title for the collection
      responses:
        200:
          description: OK
      tags:
      - Collections
      - :id
  /comments/:id/comments:
    post:
      summary: Post Comments Comments
      description: Creates a reply to an existing comment. Comments can only be nested
        one level deep, you cannot reply to a reply of a comment. If a comment has
        a non-null parent_id value then it cannot be replied to.
      operationId: creates-a-reply-to-an-existing-comment-comments-can-only-be-nested-one-level-deep-you-cannot-reply-t
      x-api-path-slug: commentsidcomments-post
      parameters:
      - in: query
        name: body (required)
        description: Content of the comment
      responses:
        200:
          description: OK
      tags:
      - Comments
      - :id
      - Comments
  /photos:
    post:
      summary: Post Photos
      description: Create a new photo on behalf of the user, and receive an upload
        key in exchange.
      operationId: create-a-new-photo-on-behalf-of-the-user-and-receive-an-upload-key-in-exchange
      x-api-path-slug: photos-post
      parameters:
      - in: query
        name: aperture
        description: Aperture value
      - in: query
        name: camera
        description: Make and model of the camera
      - in: query
        name: category
        description: A numerical ID for the Category of the photo
      - in: query
        name: description
        description: Description for the photo
      - in: query
        name: focal_length
        description: Focal length in millimetres, a string representing an integer
          value
      - in: query
        name: iso
        description: ISO value
      - in: query
        name: latitude
        description: Latitude, in decimal format
      - in: query
        name: lens
        description: Lens used to make this photo
      - in: query
        name: longitude
        description: Longitude, in decimal format
      - in: query
        name: name
        description: Title of the photo
      - in: query
        name: privacy
        description: Whether to hide the photo from the user profile on the website
      - in: query
        name: shutter_speed
        description: Shutter speed in seconds, represented by string containing a
          rational expression if the value is 1sec
      - in: query
        name: tags
        description: Comma-separated list of tags to apply to the photo
      responses:
        200:
          description: OK
      tags:
      - Photos
  /photos/:id:
    put:
      summary: Put Photos
      description: 'Allows the client application to update user-editable information
        on a photo.nnnResource URLnnhttps://api.500px.com/v1/photos/:idnnnnAuthenticationnnRequired;
        OAuth. The client application must use the OAuth access token issued for the
        owner of the photo to access this resouce.nnnParametersnnThe application must
        provide the ID of the photo to update in the URL of the request. The following
        parameters are recognized when included in the query string or POST body:nnnnname:
        Title of the photo, up to 255 characters in length.nndescription: Text description
        of the photo, up to 65535 characters in length.nncategory: Integer number
        of the category of the photo. See category mapping for exact values.nntags:
        Comma-separated list of tags applicable to this photo.nnadd_tags: Comma-separated
        list of tags to add to this photos existing tags.nnremove_tags: Comma-separated
        list of tags to remove from this photos existing tags.nnshutter_speed: Shutter
        speed value for the photo, internally stored as string.nnfocal_length: Focal
        length value for the photo, internally stored as string.nnaperture: Aperture
        value value for the photo, internally stored as string.nniso: Integer ISO
        value for the photo.nncamera: Make and model of the camera used to take this
        photo.nnlens: Information about the lens used to take this photo.nnlatitude:
        Latitude of the location this photo was taken at represented by a decimal
        number.nnlongitude: Longitude of the location this photo was taken at represented
        by a decimal number.nnnsfw: Boolean value indicating that the photo may contain
        not-safe-for-work content or content not suitable for minors.nnlicense_type:
        Integer number of the license type chosen for this photo. See license type
        mapping for exact values.nnprivacy: Integer value indicating that the photo
        should be shown (0) or hidden (1) on the users profile.nncrop: A hash containing
        keys x, x2, y, y2 and representing coordinates within which the thumbnail
        must be cropped. The crop is made using the top left corner as the origin.
        The points must be given relative to image size 4, an image of at most 900px
        on the larger side. The client application may skip this if the user does
        not wish to change photo thumbnail.nnnnImplementation detailsnnA parameter
        missing from the request will not be updated.  A parameter set to an empty
        string or null value will be interpreted as the user wishing to reset the
        value of the field to its default value.nnYou can use the add_tags and remove_tags
        parameters to manupulate a photos tags without having to send the complete
        list of tags in the request.nnnReturn formatnnA JSON object containing key
        photo, where photo is a Photo object in full format.nnnErrorsnnAll known errors
        cause the resource to return HTTP error code header together with a JSON array
        containing at least status and error keys describing the source of error.nnnn401:
        Invalid OAuth request: The request was refused because the OAuth signature
        is incorrect.nn404: Photo with ID not found: The photo ID provided is not
        known to the system.nn404: Photo with ID has been deleted: The photo has been
        deleted and can not be edited.nn404: Photo with ID belongs to a deactivated
        user: The photo belongs to a user that is no longer active and can not be
        edited.nn400: Bad photo category: An unrecognized photo category value has
        been provided.nn400: Bad license type: An unrecognized license type value
        has been provided.'
      operationId: allows-the-client-application-to-update-usereditable-information-on-a-photoresource-urlhttpsapi500px
      x-api-path-slug: photosid-put
      parameters:
      - in: query
        name: 'add_tags: Comma-separated list of tags to add to this photos existing
          tags.'
      - in: query
        name: 'aperture: Aperture value value for the photo, internally stored as
          string.'
      - in: query
        name: 'camera: Make and model of the camera used to take this photo.'
      - in: query
        name: 'category: Integer number of the category of the photo. See category
          mapping for exact values.'
      - in: query
        name: 'crop: A hash containing keys x, x2, y, y2 and representing coordinates
          within which the thumbnail must be cropped. The crop is made using the top
          left corner as the origin. The points must be given relative to image size
          4, an image of at most 900px'
      - in: query
        name: 'description: Text description of the photo, up to 65535 characters
          in length.'
      - in: query
        name: 'focal_length: Focal length value for the photo, internally stored as
          string.'
      - in: query
        name: 'iso: Integer ISO value for the photo.'
      - in: query
        name: 'latitude: Latitude of the location this photo was taken at represented
          by a decimal number.'
      - in: query
        name: 'lens: Information about the lens used to take this photo.'
      - in: query
        name: 'license_type: Integer number of the license type chosen for this photo.
          See license type mapping for exact values.'
      - in: query
        name: 'longitude: Longitude of the location this photo was taken at represented
          by a decimal number.'
      - in: query
        name: 'name: Title of the photo, up to 255 characters in length.'
      - in: query
        name: 'nsfw: Boolean value indicating that the photo may contain not-safe-for-work
          content or content not suitable for minors.'
      - in: query
        name: 'privacy: Integer value indicating that the photo should be shown (0)
          or hidden (1) on the users profile.'
      - in: query
        name: 'remove_tags: Comma-separated list of tags to remove from this photos
          existing tags.'
      - in: query
        name: 'shutter_speed: Shutter speed value for the photo, internally stored
          as string.'
      - in: query
        name: 'tags: Comma-separated list of tags applicable to this photo.'
      responses:
        200:
          description: OK
      tags:
      - Photos
      - :id
  /photos/:id/comments:
    post:
      summary: Post Photos Comments
      description: Creates a new comment for the photo.
      operationId: creates-a-new-comment-for-the-photo
      x-api-path-slug: photosidcomments-post
      parameters:
      - in: query
        name: body (required)
        description: Content of the comment
      - in: query
        name: id (required)
        description: The Photo ID to post comments for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - :id
      - Comments
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