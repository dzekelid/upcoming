---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
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
---