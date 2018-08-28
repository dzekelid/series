---
name: Google Books
x-slug: google-books
description: Google Books is our effort to make book content more discoverable on
  the Web. Using the Google Books API, your application can perform full-text searches
  and retrieve book information, viewability and eBook availability. You can also
  manage your personal bookshelves.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
  Shot 2017-03-16 at 4.28.26 PM.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Series
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/google-books/apis.md
specificationVersion: "0.14"
apis:
- name: Books - Get Series
  x-api-slug: seriesget-get
  description: Returns Series metadata for the given series ids.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/google-books/seriesget-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/google-books/seriesget-get-openapi.md
- name: Books - Get Series Membership
  x-api-slug: seriesmembershipget-get
  description: Returns Series membership data given the series id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 4.28.26 PM.png
  humanURL: https://developers.google.com/books/
  baseURL: ://www.googleapis.com//books/v1
  tags: Books, Google APIs, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/google-books/seriesmembershipget-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/google-books/seriesmembershipget-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.biquery.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.books.stack.network
- type: x-blog
  url: http://booksearch.blogspot.com
- type: x-blog-rss
  url: http://booksearch.blogspot.com/feeds/posts/default?alt=rss
- type: x-branding-guidelines
  url: https://developers.google.com/books/branding
- type: x-code
  url: https://developers.google.com/books/docs/v1/libraries
- type: x-documentation
  url: https://developers.google.com/books/docs/overview
- type: x-embeddable
  url: https://developers.google.com/books/docs/viewer/developers_guide
- type: x-partners
  url: https://books.google.com/intl/en/googlebooks/partners/
- type: x-privacy-policy
  url: https://books.google.com/intl/en/policies/privacy/
- type: x-terms-of-service
  url: https://developers.google.com/books/terms.html
- type: x-website
  url: https://developers.google.com/books/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---