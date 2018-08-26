---
swagger: "2.0"
x-collection-name: Rotten Tomatoes
x-complete: 1
info:
  title: Rotten Tomatoes
  description: test-our-api-services-using-io-docs-
  contact:
    name: Mike Ralphson
    url: https://github.com/mermade/mashery2openapi
    email: mike.ralphson@gmail.com
  version: "1.0"
host: api.rottentomatoes.com
basePath: /api/public/v1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lists/dvds/upcoming.json:
    get:
      summary: Get Lists Dvds Upcoming
      description: Get lists dvds upcoming.json.
      operationId: getListsDvdsUpcoming.json
      x-api-path-slug: listsdvdsupcoming-json-get
      parameters:
      - in: query
        name: country
        description: Provides localized data for the selected country (ISO 3166-1
          alpha-2) if available
      - in: query
        name: page
        description: The selected page of upcoming DVDs
      - in: query
        name: page_limit
        description: The amount of upcoming dvds to show per page
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Dvds
      - Upcoming
  /lists/movies/upcoming.json:
    get:
      summary: Get Lists Movies Upcoming
      description: Get lists movies upcoming.json.
      operationId: getListsMoviesUpcoming.json
      x-api-path-slug: listsmoviesupcoming-json-get
      parameters:
      - in: query
        name: country
        description: Provides localized data for the selected country (ISO 3166-1
          alpha-2) if available
      - in: query
        name: page
        description: The selected page of upcoming movies
      - in: query
        name: page_limit
        description: The amount of upcoming movies to show per page
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Movies
      - Upcoming
---