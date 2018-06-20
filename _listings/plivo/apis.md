---
name: Plivo
x-slug: plivo
description: 'Voice & SMS API Platform: Plivo enables businesses and developers to
  tap into powerful Voice and SMS capabilities without carrier lock-in.'
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
x-kinRank: "8"
x-alexaRank: "116335"
tags: Plivo
created: "2018-06-19"
modified: "2018-06-19"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/apis.md
specificationVersion: "0.14"
apis:
- name: Codenvy Account API Get Account
  x-api-slug: codenvy-account-api
  description: This API call returns a JSON with all user membership in a single or
    multiple accounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//account
  tags: Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/account-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/account-get-openapi.md
- name: Codenvy Account API Post Account
  x-api-slug: codenvy-account-api
  description: Create a new account
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//account
  tags: Account
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/account-post-openapi.md
- name: Codenvy Account API Get Account Find
  x-api-slug: codenvy-account-api
  description: Get account information by its name. JSON with account details is returned.
    This API call requires system/admin or system/manager role.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//account/find
  tags: Account,Find
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/accountfind-get-openapi.md
- name: Codenvy Account API Get Account Memberships
  x-api-slug: codenvy-account-api
  description: ID of a user should be specified as a query parameter. JSON with membership
    details is returned. For this API call system/admin or system/manager role is
    required
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//account/memberships
  tags: Account,Memberships
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/accountmemberships-get-openapi.md
- name: Codenvy Account API Post Account Subscriptions
  x-api-slug: codenvy-account-api
  description: 'Add a new subscription to an account. JSON with subscription details
    is sent. Roles: account/owner, system/admin.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//account/subscriptions
  tags: Account,Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/accountsubscriptions-post-openapi.md
- name: Codenvy Account API Delete Account Subscriptions Subscriptionid
  x-api-slug: codenvy-account-api
  description: 'Remove subscription from account. Roles: account/owner, system/admin.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//account/subscriptions/{subscriptionId}
  tags: Account,Subscriptions,SubscriptionId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/accountsubscriptionssubscriptionid-delete-openapi.md
- name: Codenvy Account API Get Account Subscriptions Subscriptionid
  x-api-slug: codenvy-account-api
  description: Get information on a particular subscription by its unique ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//account/subscriptions/{subscriptionId}
  tags: Account,Subscriptions,SubscriptionId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/accountsubscriptionssubscriptionid-get-openapi.md
- name: Codenvy Account API Get Account Accountid Subscriptions
  x-api-slug: codenvy-account-api
  description: Get information on account subscriptions. This API call requires account/owner,
    account/member, system/admin or system/manager role.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//account/{accountId}/subscriptions
  tags: Account,AccountId,Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/accountaccountidsubscriptions-get-openapi.md
- name: Codenvy Account API Delete Account
  x-api-slug: codenvy-account-api
  description: Remove subscription from account. JSON with subscription details is
    sent. Can be performed only by system/admin.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//account/{id}
  tags: Account,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/accountid-delete-openapi.md
- name: Codenvy Account API Get Account
  x-api-slug: codenvy-account-api
  description: Get account information by its ID. JSON with account details is returned.
    This API call requires account/owner, system/admin or system/manager role.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//account/{id}
  tags: Account,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/accountid-get-openapi.md
- name: Codenvy Account API Post Account
  x-api-slug: codenvy-account-api
  description: Update account. This API call requires account/owner role.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//account/{id}
  tags: Account,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/accountid-post-openapi.md
- name: Codenvy Account API Delete Account Attribute
  x-api-slug: codenvy-account-api
  description: Remove attribute from an account. Attribute name is used as a quary
    parameter. For this API request account/owner, system/admin or system/manager
    role is required
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//account/{id}/attribute
  tags: Account,Id,Attribute
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/accountidattribute-delete-openapi.md
- name: Codenvy Account API Get Account Members
  x-api-slug: codenvy-account-api
  description: Get all members for a specific account. This API call requires account/owner,
    system/admin or system/manager role.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//account/{id}/members
  tags: Account,Id,Members
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/accountidmembers-get-openapi.md
- name: Codenvy Account API Post Account Members
  x-api-slug: codenvy-account-api
  description: Add a new user to an account. This user will have account/member role.
    This API call requires account/owner, system/admin or system/manager role.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//account/{id}/members
  tags: Account,Id,Members
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/accountidmembers-post-openapi.md
- name: Codenvy Account API Delete Account Members User
  x-api-slug: codenvy-account-api
  description: Remove user from a specific account. This API call requires account/owner,
    system/admin or system/manager role.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//account/{id}/members/{userid}
  tags: Account,Id,Members,Userid
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/accountidmembersuserid-delete-openapi.md
- name: Codenvy Account API Get Account Resources
  x-api-slug: codenvy-account-api
  description: 'Returns used resources, provided by subscriptions. Roles: account/owner,
    account/member, system/manager, system/admin.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//account/{id}/resources
  tags: Account,Id,Resources
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/accountidresources-get-openapi.md
- name: Codenvy Account API Post Account Resources
  x-api-slug: codenvy-account-api
  description: 'Redistributes resources between workspaces. Roles: account/owner,
    system/manager, system/admin.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//account/{id}/resources
  tags: Account,Id,Resources
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/accountidresources-post-openapi.md
- name: Codenvy Account API Post Blogs
  x-api-slug: codenvy-account-api
  description: Creates a new Story.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//blogs/
  tags: Blogs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/blogs-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/blogs-post-openapi.md
- name: Codenvy Account API Put Blogs
  x-api-slug: codenvy-account-api
  description: Updates the Story.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//blogs/:id
  tags: Blogs,:id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/blogsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/blogsid-put-openapi.md
- name: Codenvy Account API Post Blogs Comments
  x-api-slug: codenvy-account-api
  description: Creates a comment for the Story.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//blogs/:id/comments
  tags: Blogs,:id,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/blogsidcomments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/blogsidcomments-post-openapi.md
- name: Codenvy Account API Post Collections
  x-api-slug: codenvy-account-api
  description: Creates new a collection.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//collections
  tags: Collections
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/collections-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/collections-post-openapi.md
- name: Codenvy Account API Put Collections
  x-api-slug: codenvy-account-api
  description: Updates collection.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//collections/:id
  tags: Collections,:id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/collectionsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/collectionsid-put-openapi.md
- name: Codenvy Account API Post Comments Comments
  x-api-slug: codenvy-account-api
  description: Creates a reply to an existing comment. Comments can only be nested
    one level deep, you cannot reply to a reply of a comment. If a comment has a non-null
    parent_id value then it cannot be replied to.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//comments/:id/comments
  tags: Comments,:id,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/commentsidcomments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/commentsidcomments-post-openapi.md
- name: Codenvy Account API Post Photos
  x-api-slug: codenvy-account-api
  description: Create a new photo on behalf of the user, and receive an upload key
    in exchange.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//photos
  tags: Photos
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/photos-post-openapi.md
- name: Codenvy Account API Put Photos
  x-api-slug: codenvy-account-api
  description: 'Allows the client application to update user-editable information
    on a photo.nnnResource URLnnhttps://api.500px.com/v1/photos/:idnnnnAuthenticationnnRequired;
    OAuth. The client application must use the OAuth access token issued for the owner
    of the photo to access this resouce.nnnParametersnnThe application must provide
    the ID of the photo to update in the URL of the request. The following parameters
    are recognized when included in the query string or POST body:nnnnname: Title
    of the photo, up to 255 characters in length.nndescription: Text description of
    the photo, up to 65535 characters in length.nncategory: Integer number of the
    category of the photo. See category mapping for exact values.nntags: Comma-separated
    list of tags applicable to this photo.nnadd_tags: Comma-separated list of tags
    to add to this photos existing tags.nnremove_tags: Comma-separated list of tags
    to remove from this photos existing tags.nnshutter_speed: Shutter speed value
    for the photo, internally stored as string.nnfocal_length: Focal length value
    for the photo, internally stored as string.nnaperture: Aperture value value for
    the photo, internally stored as string.nniso: Integer ISO value for the photo.nncamera:
    Make and model of the camera used to take this photo.nnlens: Information about
    the lens used to take this photo.nnlatitude: Latitude of the location this photo
    was taken at represented by a decimal number.nnlongitude: Longitude of the location
    this photo was taken at represented by a decimal number.nnnsfw: Boolean value
    indicating that the photo may contain not-safe-for-work content or content not
    suitable for minors.nnlicense_type: Integer number of the license type chosen
    for this photo. See license type mapping for exact values.nnprivacy: Integer value
    indicating that the photo should be shown (0) or hidden (1) on the users profile.nncrop:
    A hash containing keys x, x2, y, y2 and representing coordinates within which
    the thumbnail must be cropped. The crop is made using the top left corner as the
    origin. The points must be given relative to image size 4, an image of at most
    900px on the larger side. The client application may skip this if the user does
    not wish to change photo thumbnail.nnnnImplementation detailsnnA parameter missing
    from the request will not be updated.  A parameter set to an empty string or null
    value will be interpreted as the user wishing to reset the value of the field
    to its default value.nnYou can use the add_tags and remove_tags parameters to
    manupulate a photos tags without having to send the complete list of tags in the
    request.nnnReturn formatnnA JSON object containing key photo, where photo is a
    Photo object in full format.nnnErrorsnnAll known errors cause the resource to
    return HTTP error code header together with a JSON array containing at least status
    and error keys describing the source of error.nnnn401: Invalid OAuth request:
    The request was refused because the OAuth signature is incorrect.nn404: Photo
    with ID not found: The photo ID provided is not known to the system.nn404: Photo
    with ID has been deleted: The photo has been deleted and can not be edited.nn404:
    Photo with ID belongs to a deactivated user: The photo belongs to a user that
    is no longer active and can not be edited.nn400: Bad photo category: An unrecognized
    photo category value has been provided.nn400: Bad license type: An unrecognized
    license type value has been provided.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//photos/:id
  tags: Photos,:id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/photosid-put-openapi.md
- name: Codenvy Account API Post Photos Comments
  x-api-slug: codenvy-account-api
  description: Creates a new comment for the photo.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//photos/:id/comments
  tags: Photos,:id,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/photosidcomments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/photosidcomments-post-openapi.md
- name: Codenvy Account API Post Photos Favorite
  x-api-slug: codenvy-account-api
  description: Adds the photo to users list of favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//photos/:id/favorite
  tags: Photos,:id,Favorite
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/photosidfavorite-post-openapi.md
- name: Codenvy Account API Get Photos Favorites
  x-api-slug: codenvy-account-api
  description: Returns all users that had favorite that photo.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//photos/:id/favorites
  tags: Photos,:id,Favorites
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/photosidfavorites-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/photosidfavorites-get-openapi.md
- name: Codenvy Account API Post Photos Report
  x-api-slug: codenvy-account-api
  description: Allows to report a photo.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//photos/:id/report
  tags: Photos,:id,Report
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/photosidreport-post-openapi.md
- name: Codenvy Account API Post Photos Tags
  x-api-slug: codenvy-account-api
  description: Adds tags to the photo. Accepts one or multiple coma separated tags.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//photos/:id/tags
  tags: Photos,:id,Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/photosidtags-post-openapi.md
- name: Codenvy Account API Post Photos Vote
  x-api-slug: codenvy-account-api
  description: Allows the user to vote for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//photos/:id/vote
  tags: Photos,:id,Vote
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/photosidvote-post-openapi.md
- name: Codenvy Account API Get Photos Votes
  x-api-slug: codenvy-account-api
  description: Returns all users that had liked this photo.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//photos/:id/votes
  tags: Photos,:id,Votes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/photosidvotes-get-openapi.md
- name: Codenvy Account API Get Photos Search
  x-api-slug: codenvy-account-api
  description: Returns a listing of twenty (up to one hundred) photos from search
    results for a specified tag, keyword, or location.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//photos/search
  tags: Photos,Search
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/photossearch-get-openapi.md
- name: Codenvy Account API Post Photos Upload
  x-api-slug: codenvy-account-api
  description: This is a new photo upload endpoint. It is currently in beta.nCreate
    a new photo on behalf of the user and upload a file.nfile parameter is passed
    in multipart/form-data, other parameters are passed as query parametrs or multipart/form-data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//photos/upload
  tags: Photos,Upload
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/photosupload-post-openapi.md
- name: Codenvy Account API Post Upload
  x-api-slug: codenvy-account-api
  description: Allows an application to upload the photo file.nnNote that this endpoint
    is at the upload.500px.com domain, not the api.500px.com domain.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//upload
  tags: Upload
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/upload-post-openapi.md
- name: Codenvy Account API Get Users
  x-api-slug: codenvy-account-api
  description: Returns the profile information for the current user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//users
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/users-get-openapi.md
- name: Codenvy Account API Get Users Followers
  x-api-slug: codenvy-account-api
  description: Returns a list of users who follow the specified user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//users/:id/followers
  tags: Users,:id,Followers
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/usersidfollowers-get-openapi.md
- name: Codenvy Account API Post Users Friends
  x-api-slug: codenvy-account-api
  description: Add the user to the list of followers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//users/:id/friends
  tags: Users,:id,Friends
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/usersidfriends-post-openapi.md
- name: Codenvy Account API Get Users Search
  x-api-slug: codenvy-account-api
  description: Return listing of ten (up to one hundred) users from search results
    for a specified search term.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//users/search
  tags: Users,Search
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/userssearch-get-openapi.md
- name: Codenvy Account API Get Users Show
  x-api-slug: codenvy-account-api
  description: Returns the profile information for a specified user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api//users/show
  tags: Users,Show
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/usersshow-get-openapi.md
- name: Codenvy Account API
  x-api-slug: codenvy-account-api
  description: 'Voice & SMS API Platform: Plivo enables businesses and developers
    to tap into powerful Voice and SMS capabilities without carrier lock-in.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api
  tags: Plivo
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/openapi.md
- name: Plivo SMS Message
  x-api-slug: plivo-sms
  description: Get details of a message.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: https://api.plivo.com/v1//{auth_id}/Message/
  tags: Message
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/auth-idmessage-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/auth-idmessage-get-openapi.md
- name: Plivo SMS Send Message
  x-api-slug: plivo-sms
  description: This API enables you to send messages via Plivou2019s SMS service.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: https://api.plivo.com/v1//{auth_id}/Message/
  tags: Send,Message
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/auth-idmessage-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/auth-idmessage-post-openapi.md
- name: Plivo SMS Message
  x-api-slug: plivo-sms
  description: Get details of a single message.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: https://api.plivo.com/v1//{auth_id}/Message/{message_uuid}/
  tags: Message
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/auth-idmessagemessage-uuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/auth-idmessagemessage-uuid-get-openapi.md
- name: Plivo SMS
  x-api-slug: plivo-sms
  description: Plivo provides web developers with basic building blocks in the form
    of Plivo XML and HTTP API, to create telephony apps, so developers can completely
    do away with learning the nitty-gritty of the telephony plumbing.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: https://api.plivo.com/v1/
  tags: Plivo
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/plivo/master/_listings/plivo/openapi.md
x-common:
- type: x--net-library
  url: https://www.plivo.com/docs/helpers/dotnet/
- type: x-android-sdk
  url: https://www.plivo.com/docs/sdk/android/
- type: x-base
  url: https://api.plivo.com
- type: x-blog
  url: http://blog.plivo.com
- type: x-blog-rss
  url: http://blog.plivo.com/rss
- type: x-crunchbase
  url: https://crunchbase.com/organization/plivo
- type: x-crunchbase
  url: http://www.crunchbase.com/company/plivo
- type: x-documentation
  url: https://plivo.com/docs/
- type: x-email
  url: marketing@plivo.com
- type: x-email
  url: legalrequests@plivo.com
- type: x-email
  url: privacy@plivo.com
- type: x-faq
  url: https://plivo.com/faq/
- type: x-github
  url: https://github.com/plivo
- type: x-ios-sdk
  url: https://www.plivo.com/docs/sdk/ios/
- type: x-java-sdk
  url: https://www.plivo.com/docs/helpers/java/
- type: x-node-js-library
  url: https://www.plivo.com/docs/helpers/node/
- type: x-php-sdk
  url: https://www.plivo.com/docs/helpers/php/
- type: x-pricing
  url: https://plivo.com/pricing/
- type: x-privacy
  url: https://plivo.com/privacy/
- type: x-ruby-library
  url: https://www.plivo.com/docs/helpers/python
- type: x-selfservice-registration
  url: https://manage.plivo.com/accounts/register/
- type: x-status
  url: https://status.plivo.com/
- type: x-terms-of-service
  url: https://plivo.com/terms/
- type: x-twitter
  url: https://twitter.com/#!/plivo
- type: x-website
  url: http:///account
- type: x-website
  url: http://plivo.com
- type: x-website
  url: https://www.plivo.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---