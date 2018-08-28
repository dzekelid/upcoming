swagger: "2.0"
x-collection-name: GoToMeeting
x-complete: 1
info:
  title: SCIM
  description: the-scim-api-lets-you-manage-users-in-your-organization--you-can-then-automate-the-provisioning-of-product-licenses-for-these-users-and-they-can-use-your-companys-single-signon-solution-through-an-identity-provider-
  termsOfService: https://developer.citrixonline.com/terms-use
  contact:
    name: Developer Support
    url: https://developer.citrixonline.com
    email: developer-support@citrixonline.com
  version: N/A
host: api.citrixonline.com
basePath: /identity/v1
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
  /organizers/{organizerKey}/upcomingWebinars:
    get:
      summary: Get upcoming webinars
      description: Returns webinars scheduled for the future for the specified organizer
        and webinars of other organizers where the specified organizer is a co-organizer.
      operationId: getUpcomingWebinars
      x-api-path-slug: organizersorganizerkeyupcomingwebinars-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - UpcomingWebinars