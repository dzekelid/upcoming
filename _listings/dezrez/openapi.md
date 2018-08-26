---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/people/unsubscribe/{id}:
    post:
      summary: Unsubscribe/Subscribe All contact items for a person
      description: Unsubscribe/subscribe all contact items for a person.
      operationId: People_UnsubscibedContactItemsByidByitems
      x-api-path-slug: apipeopleunsubscribeid-post
      parameters:
      - in: path
        name: id
      - in: body
        name: items
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Unsubscribe
      - Subscribe
      - ""
      - Contact
      - Itemsa
      - Person
---