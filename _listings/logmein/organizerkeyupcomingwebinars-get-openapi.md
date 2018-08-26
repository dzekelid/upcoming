---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 0
info:
  title: GoToWebinar Upcoming Webinars
  description: Returns webinars scheduled for the future for the specified organizer
    and webinars of other organizers where the specified organizer is a co-organizer.
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