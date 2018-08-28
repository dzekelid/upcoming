swagger: "2.0"
x-collection-name: Mailgun
x-complete: 1
info:
  title: Mailgun API
  description: powerful-apis-that-allow-you-to-send-receive-and-track-email-effortlessly-
  version: v2
host: api.mailgun.net
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  unsubscribes/:
    post:
      summary: Add to unsubscribe list.
      description: Adds address to unsubscribed table.
      operationId: postUnsubscribes
      x-api-path-slug: unsubscribes-post
      parameters:
      - in: query
        name: address
        description: The address to add to unsubscribe list
      - in: query
        name: tag
        description: Tag to unsubscribe from, use * to unsubscribe address from domain
      responses:
        200:
          description: OK
      tags:
      - To
      - Unsubscribe
      - List
  unsubscribes/{address}:
    delete:
      summary: Delete Unsubscribe
      description: Removes an address from the unsubscribes table. Address defines
        which events to delete.
      operationId: deleteUnsubscribesAddress
      x-api-path-slug: unsubscribesaddress-delete
      parameters:
      - in: query
        name: address
        description: The email address of the person on the unsubscribe list
      responses:
        200:
          description: OK
      tags:
      - Unsubscribe
    get:
      summary: Unsubscribe
      description: Retreives a single unsubscribe record. Can be used to check if
        a given address is present in the list of unsubscribed users.
      operationId: getUnsubscribesAddress
      x-api-path-slug: unsubscribesaddress-get
      parameters:
      - in: query
        name: address
        description: The email address of the person on the unsubscribe list
      responses:
        200:
          description: OK
      tags:
      - Unsubscribe