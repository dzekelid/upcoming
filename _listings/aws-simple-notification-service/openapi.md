swagger: "2.0"
x-collection-name: AWS Simple Notification Service
x-complete: 1
info:
  title: AWS Simple Notification Service API
  version: 1.0.0
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