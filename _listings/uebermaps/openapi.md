---
swagger: "2.0"
x-collection-name: uebermaps
x-complete: 1
info:
  title: uebermaps
  description: enable-people-to-store-spots-on-public-and-private-maps
  termsOfService: https://uebermaps.com/terms/
  contact:
    name: uebermaps API Team
  version: "2.0"
host: uebermaps.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /maps/{id}/subscriptions:
    delete:
      summary: Unsubscribe from map
      description: Unsubscribe from map.
      operationId: maps.id.subscriptions.delete
      x-api-path-slug: mapsidsubscriptions-delete
      parameters:
      - in: path
        name: id
        description: map id
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Unsubscribe
      - From
      - Map
---