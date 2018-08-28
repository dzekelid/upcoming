swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 1
info:
  title: GoToWebinar API
  description: todo-add-description
  version: 1.0.0
host: api.getgo.com
basePath: /G2W/rest/organizers
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/{groupKey}/upcomingMeetings:
    get:
      summary: Upcoming meetings by group
      description: Get upcoming meetings for a specified group. This API call is only
        available to users with the admin role. This API call can be used only for
        groups with maximum 50 organizers.
      operationId: GroupsUpcomingMeetingsByGroupKeyGet
      x-api-path-slug: groupsgroupkeyupcomingmeetings-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: groupKey
      responses:
        200:
          description: OK
      tags:
      - Upcoming
      - Meetings
      - By
      - Group
  /upcomingMeetings:
    get:
      summary: Upcoming meetings
      description: Gets upcoming meetings for the current authenticated organizer.
      operationId: UpcomingMeetingsGet
      x-api-path-slug: upcomingmeetings-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Upcoming
      - Meetings
  /{organizerKey}/upcomingWebinars:
    get:
      summary: Upcoming Webinars
      description: Returns webinars scheduled for the future for the specified organizer
        and webinars of other organizers where the specified organizer is a co-organizer.
      operationId: UpcomingWebinarsByOrganizerKeyGet
      x-api-path-slug: organizerkeyupcomingwebinars-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      responses:
        200:
          description: OK
      tags:
      - Upcoming
      - Webinars