---
swagger: "2.0"
x-collection-name: AWS Simple Notification Service
x-complete: 0
info:
  title: AWS Simple Notification Service API Unsubscribe
  version: 1.0.0
  description: Deletes a subscription.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=Unsubscribe:
    get:
      summary: Unsubscribe
      description: Deletes a subscription.
      operationId: unsubscribe
      x-api-path-slug: actionunsubscribe-get
      parameters:
      - in: query
        name: SubscriptionArn
        description: The ARN of the subscription to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - ""
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