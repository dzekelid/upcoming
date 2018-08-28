---
name: Rotten Tomatoes
x-slug: rotten-tomatoes
description: Rotten Tomatoes is a website launched in August 1998 devoted to film
  reviews and news; it is widely known as a film review aggregator. Coverage now includes
  TV content as well. The name derives from the practice of audiences throwing rotten
  tomatoes when disapproving of a poor stage performance. The company was created
  by Senh Duong and since January 2010 has been owned by Flixster, which itself was
  acquired in 2011 by Warner Bros.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/rotten-tomatoes-logo.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Upcoming
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/upcoming/master/_listings/rotten-tomatoes/apis.md
specificationVersion: "0.14"
apis:
- name: Rotten Tomatoes - Get Lists Dvds Upcoming
  x-api-slug: listsdvdsupcoming-json-get
  description: Get lists dvds upcoming.json.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/rotten-tomatoes-logo.png
  humanURL: http://rottentomatoes.com
  baseURL: https://api.rottentomatoes.com//api/public/v1.0
  tags: Movies, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/upcoming/master/_listings/rotten-tomatoes/listsdvdsupcoming-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/upcoming/master/_listings/rotten-tomatoes/listsdvdsupcoming-json-get-openapi.md
- name: Rotten Tomatoes - Get Lists Movies Upcoming
  x-api-slug: listsmoviesupcoming-json-get
  description: Get lists movies upcoming.json.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/rotten-tomatoes-logo.png
  humanURL: http://rottentomatoes.com
  baseURL: https://api.rottentomatoes.com//api/public/v1.0
  tags: Movies, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/upcoming/master/_listings/rotten-tomatoes/listsmoviesupcoming-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/upcoming/master/_listings/rotten-tomatoes/listsmoviesupcoming-json-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://rite.kit.api.gallery.streamdata.io
- type: x-api-stack
  url: http://rotten.tomatoes.stack.network
- type: x-developer
  url: http://developer.rottentomatoes.com/
- type: x-twitter
  url: https://twitter.com/RottenTomatoes
- type: x-website
  url: http://rottentomatoes.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---