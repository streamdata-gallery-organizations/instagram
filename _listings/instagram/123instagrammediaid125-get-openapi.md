---
swagger: "2.0"
x-collection-name: Instagram
x-complete: 0
info:
  title: Instagram Instagram Media
  version: 1.0.0
  description: Instagram Media
host: graph.facebook.com
basePath: /v3.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /&#123;instagram-media-id&#125;/comments:
    get:
      summary: Instagram Media Comments
      description: Instagram Media Comments
      operationId: getInstagramMediaComments
      x-api-path-slug: 123instagrammediaid125comments-get
      parameters:
      - in: query
        name: "100"
        description: Invalid parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instagram
      - Media
      - Comments
  /&#123;instagram-user-id&#125;:
    get:
      summary: Instagram User
      description: Instagram User
      operationId: getInstagramUser
      x-api-path-slug: 123instagramuserid125-get
      parameters:
      - in: query
        name: followed_by_countint32
        description: Number of Instagram users that follow this Instagram user
        type: string
      - in: query
        name: follow_countint32
        description: Number of Instagram users that this Instagram user follows
        type: string
      - in: query
        name: has_profile_picturebool
        description: Indicates whether Instagram Account has a profile picture
        type: string
      - in: query
        name: idnumeric string
        description: ID of the Instagram user
        type: string
      - in: query
        name: is_privatebool
        description: Whether the Instagram user is private
        type: string
      - in: query
        name: is_publishedbool
        description: Whether the Instagram user is published
        type: string
      - in: query
        name: media_countint32
        description: Number of active media posted by this Instagram user
        type: string
      - in: query
        name: profile_picstring
        description: URI to user&#039;s Instagram profile picture
        type: string
      - in: query
        name: usernamestring
        description: Instagram username
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instagram
      - User
  /&#123;instagram-user-id&#125;/agencies:
    get:
      summary: Instagram User Agencies
      description: Instagram User Agencies
      operationId: getInstagramUserAgencies
      x-api-path-slug: 123instagramuserid125agencies-get
      parameters:
      - in: query
        name: "294"
        description: Managing advertisements requires an access token with the extended
          permission for ads_management
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instagram
      - User
      - Agencies
  /&#123;instagram-user-id&#125;/authorized_adaccounts:
    get:
      summary: Instagram User Authorized Adaccounts
      description: Instagram User Authorized Adaccounts
      operationId: getInstagramUserAuthorizedAdaccounts
      x-api-path-slug: 123instagramuserid125authorized-adaccounts-get
      parameters:
      - in: query
        name: "100"
        description: Invalid parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instagram
      - User
      - Authorized
      - Adaccounts
  /&#123;instagram-media-id&#125;:
    get:
      summary: Instagram Media
      description: Instagram Media
      operationId: getInstagramMedia
      x-api-path-slug: 123instagrammediaid125-get
      parameters:
      - in: query
        name: caption_textstring
        description: Caption text
        type: string
      - in: query
        name: comment_countint32
        description: Number of comments
        type: string
      - in: query
        name: content_typeint32
        description: 0 for photo, 1 for video
        type: string
      - in: query
        name: display_urlstring
        description: URL of the photo or cover frame
        type: string
      - in: query
        name: filter_namestring
        description: Name of filter
        type: string
      - in: query
        name: idnumeric string
        description: ID of the Instagram media
        type: string
      - in: query
        name: latitudefloat
        description: Latitude of the location
        type: string
      - in: query
        name: like_countint32
        description: Number of likes
        type: string
      - in: query
        name: locationLocation
        description: Location data
        type: string
      - in: query
        name: location_namestring
        description: Name of location for location tag
        type: string
      - in: query
        name: longitudefloat
        description: Longitude of the location
        type: string
      - in: query
        name: owner_instagram_userInstagramUser
        description: The Instagram user that owns this media
        type: string
      - in: query
        name: permalinkstring
        description: Link to the media page on Instagram
        type: string
      - in: query
        name: taken_atdatetime
        description: When the media was created
        type: string
      - in: query
        name: video_urlstring
        description: URL of the video
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instagram
      - Media
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