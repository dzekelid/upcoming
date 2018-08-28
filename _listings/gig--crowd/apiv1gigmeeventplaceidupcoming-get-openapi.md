---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Gigme Event Placeid Upcoming
  version: 1.0.0
  description: Get gigme event placeid upcoming.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/gigme/event/{placeId}/upcoming:
    get:
      summary: Get Gigme Event Placeid Upcoming
      description: Get gigme event placeid upcoming.
      operationId: getApiV1GigmeEventPlaceUpcoming
      x-api-path-slug: apiv1gigmeeventplaceidupcoming-get
      parameters:
      - in: path
        name: placeId
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Event
      - Placeid
      - Upcoming
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