---
swagger: "2.0"
x-collection-name: GoToMeeting
x-complete: 0
info:
  title: Go To Meeting Get upcoming meetings by group
  description: Get upcoming meetings for a specified group. This API call is only
    available to users with the admin role. This API call can be used only for groups
    with maximum 50 organizers.
  termsOfService: https://developer.citrixonline.com/terms-use
  contact:
    name: Developer Support
    url: https://developer.citrixonline.com
    email: developer-support@citrixonline.com
  version: 1.0.0
host: api.citrixonline.com
basePath: /G2M/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/{groupKey}/upcomingMeetings:
    get:
      summary: Get upcoming meetings by group
      description: Get upcoming meetings for a specified group. This API call is only
        available to users with the admin role. This API call can be used only for
        groups with maximum 50 organizers.
      operationId: get-upcoming-meetings-for-a-specified-group--this-api-call-is-only-available-to-users-with-the-admin
      x-api-path-slug: groupsgroupkeyupcomingmeetings-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Groups
      - GroupKey
      - UpcomingMeetings
  /organizers/{organizerKey}/upcomingMeetings:
    get:
      summary: Get upcoming meetings by organizer
      description: Get upcoming meetings for a specified organizer. This API call
        is only available to users with the admin role.
      operationId: get-upcoming-meetings-for-a-specified-organizer--this-api-call-is-only-available-to-users-with-the-a
      x-api-path-slug: organizersorganizerkeyupcomingmeetings-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - UpcomingMeetings
  /upcomingMeetings:
    get:
      summary: Get upcoming meetings
      description: Gets upcoming meetings for the current authenticated organizer.
      operationId: gets-upcoming-meetings-for-the-current-authenticated-organizer-
      x-api-path-slug: upcomingmeetings-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - UpcomingMeetings
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