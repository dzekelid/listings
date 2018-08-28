---
name: Entertainment Express
x-slug: entertainment-express
description: Internet Video Archive (IVA) is a leading entertainment data company
  providing metadata, images and trailers/clips, for movie and TV content. With the
  launch of its award-winning Entertainment Express APIs, clients can easily access
  everything they need to create engaging content discovery experiences. By using
  Entertainment Express, clients can also connect to other services like movie showtimes
  and ticketing, content recommendations, content availability and TV channel line-ups.
  With over a million titles, episodes and over 150,000 videos available, IVA makes
  it easy for developers to integrate all the services they need at a very affordable
  price.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Listings
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/entertainment-express/apis.md
specificationVersion: "0.14"
apis:
- name: 'Entertainment Express - '
  x-api-slug: tvmedialeaguesleagueidlistings-get
  description: Retrieve listings for a given leagueID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/entertainment-express/tvmedialeaguesleagueidlistings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/entertainment-express/tvmedialeaguesleagueidlistings-get-openapi.md
- name: 'Entertainment Express - '
  x-api-slug: tvmedialineupslineupidlistings-get
  description: Retrieve individual listings for a given lineup ordered by start time
    (listDateTime) and channel number; unless using the search parameter, in which
    case they will be ordered by search term relevance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/entertainment-express/tvmedialineupslineupidlistings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/entertainment-express/tvmedialineupslineupidlistings-get-openapi.md
- name: 'Entertainment Express - '
  x-api-slug: tvmedialineupslineupidlistingsgrid-get
  description: A collection of listings grouped by channel and ordered by listDateTime.
    The grid dimensions ( time x channels ) can be modified by using the start, end,
    startchan and maxchan parameters. Channels without any listings will be returned
    with an empty listings collection.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/entertainment-express/tvmedialineupslineupidlistingsgrid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/entertainment-express/tvmedialineupslineupidlistingsgrid-get-openapi.md
- name: 'Entertainment Express - '
  x-api-slug: tvmedialineupslineupidlistingshighlights-get
  description: Retrieves featured listings. setting a start and/or end time for every
    request is a highly recommended.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/entertainment-express/tvmedialineupslineupidlistingshighlights-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/entertainment-express/tvmedialineupslineupidlistingshighlights-get-openapi.md
- name: Entertainment Express - Stations are not tied to lineups, therefore no channel
    numbers will be present in the response, unlike most other listing operations.
  x-api-slug: tvmediastationsstationidlistings-get
  description: Get listings for a given station.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/entertainment-express/tvmediastationsstationidlistings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/entertainment-express/tvmediastationsstationidlistings-get-openapi.md
- name: 'Entertainment Express - '
  x-api-slug: tvmediateamsteamidlistings-get
  description: Retrieve listings for a given TeamID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/IVA-logo.png
  humanURL: https://www.internetvideoarchive.com/
  baseURL: https://ee.iva-api.com//
  tags: Celebrities, Movies, General Data, Televisions, Videos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/entertainment-express/tvmediateamsteamidlistings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/entertainment-express/tvmediateamsteamidlistings-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://emuseum.api.docs.api.gallery.streamdata.io
- type: x-api-stack
  url: http://entertainment.express.stack.network
- type: x-blog
  url: https://www.internetvideoarchive.com/blog/
- type: x-developer
  url: https://developer.iva-api.com/
- type: x-pricing
  url: https://www.internetvideoarchive.com/pricing/
- type: x-website
  url: https://www.internetvideoarchive.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---