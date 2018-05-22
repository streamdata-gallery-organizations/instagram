---
swagger: "2.0"
x-collection-name: Instagram
x-complete: 0
info:
  title: Instagram Instagram User
  version: 1.0.0
  description: Instagram User
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
x-streamrank:
  polling_total_time_average: ~
  polling_size_download_average: ~
  streaming_total_time_average: ~
  streaming_size_download_average: ~
  change_yes: ~
  change_no: ~
  time_percentage: ~
  size_percentage: ~
  change_percentage: "200"
  last_run: ~
  days_run: ~
  minute_run: ~
---