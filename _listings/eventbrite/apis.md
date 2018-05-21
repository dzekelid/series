---
name: Eventbrite
x-slug: eventbrite
description: Eventbrite believes that anyone can be an event organizer. That&rsquo;s
  why they offer tools that make it easy to sell tickets to all kinds of events whether
  it&rsquo;s a photography class or a sold-out concert, an inspiring conference or
  an air-guitar competition. With Eventbrite, organizers can create a customizable
  event page; spread the word with social media; collect money; and gain visibility
  into attendees and sales. Eventbrite is for anyone planning or attending an event.
  It empowers event organizers to become more efficient and effective when bringing
  people together. And people everywhere are searching Eventbrite to discover great
  events that matter to them.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/eventbritelogoff8000gradient.png
x-kinRank: "9"
x-alexaRank: ""
tags: Series
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/apis.md
specificationVersion: "0.14"
apis:
- name: Eventbrite Add Series
  x-api-slug: eventbrite
  description: Creates a new repeating event series. The POST data must include information
    for at least one event date in the series.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/eventbritelogoff8000gradient.png
  humanURL: http://developer.eventbrite.com/
  baseURL: https://www.eventbriteapi.com//v3//series/
  tags: Series
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/series-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/series-post-openapi.md
- name: Eventbrite Get Series
  x-api-slug: eventbrite
  description: Returns a repeating event series parent object for the specified repeating
    event series.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/eventbritelogoff8000gradient.png
  humanURL: http://developer.eventbrite.com/
  baseURL: https://www.eventbriteapi.com//v3//series/{id}/
  tags: Series
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/seriesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/seriesid-get-openapi.md
- name: Eventbrite Add Series
  x-api-slug: eventbrite
  description: |-
    Updates a repeating event series parent object, and optionally also creates more event dates or updates or deletes
    existing event dates in the series. In order for a series date to be deleted or updated, there must be no pending or
    completed orders for that date.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/eventbritelogoff8000gradient.png
  humanURL: http://developer.eventbrite.com/
  baseURL: https://www.eventbriteapi.com//v3//series/{id}/
  tags: Series
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/seriesid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/seriesid-post-openapi.md
- name: Eventbrite Add Series  Publish
  x-api-slug: eventbrite
  description: |-
    Publishes a repeating event series and all of its occurrences that are not already canceled or deleted. Once a date is cancelled it can still be uncancelled and can be viewed by the public. A deleted date cannot be undeleted and cannot by viewed by the public. In order for
    publish to be permitted, the event must have all necessary information, including a name and description, an organizer,
    at least one ticket, and valid payment options. This API endpoint will return argument errors for event fields that
    fail to validate the publish requirements. Returns a boolean indicating success or failure of the publish.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/eventbritelogoff8000gradient.png
  humanURL: http://developer.eventbrite.com/
  baseURL: https://www.eventbriteapi.com//v3//series/{id}/publish/
  tags: Series,,Publish
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/seriesidpublish-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/seriesidpublish-post-openapi.md
- name: Eventbrite Add Series  Unpublish
  x-api-slug: eventbrite
  description: |-
    Unpublishes a repeating event series and all of its occurrences that are not already completed, canceled, or deleted. In
    order for a free series to be unpublished, it must not have any pending or completed orders for any dates, even past
    dates. In order for a paid series to be unpublished, it must not have any pending or completed orders for any dates,
    except that completed orders for past dates that have been completed and paid out do not prevent an unpublish. Returns
    a boolean indicating success or failure of the unpublish.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/eventbritelogoff8000gradient.png
  humanURL: http://developer.eventbrite.com/
  baseURL: https://www.eventbriteapi.com//v3//series/{id}/unpublish/
  tags: Series,,Unpublish
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/seriesidunpublish-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/seriesidunpublish-post-openapi.md
- name: Eventbrite Add Series  Cancel
  x-api-slug: eventbrite
  description: |-
    Cancels a repeating event series and all of its occurrences that are not already canceled or deleted. In order for
    cancel to be permitted, there must be no pending or completed orders for any dates in the series. Returns a boolean
    indicating success or failure of the cancel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/eventbritelogoff8000gradient.png
  humanURL: http://developer.eventbrite.com/
  baseURL: https://www.eventbriteapi.com//v3//series/{id}/cancel/
  tags: Series,,Cancel
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/seriesidcancel-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/seriesidcancel-post-openapi.md
- name: Eventbrite Delete Series
  x-api-slug: eventbrite
  description: |-
    Deletes a repeating event series and all of its occurrences if the delete is permitted. In order for a delete to be
    permitted, there must be no pending or completed orders for any dates in the series. Returns a boolean indicating
    success or failure of the delete.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/eventbritelogoff8000gradient.png
  humanURL: http://developer.eventbrite.com/
  baseURL: https://www.eventbriteapi.com//v3//series/{id}/
  tags: Series
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/seriesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/seriesid-delete-openapi.md
- name: Eventbrite Get Series  Events
  x-api-slug: eventbrite
  description: Returns all of the events that belong to this repeating event series.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/eventbritelogoff8000gradient.png
  humanURL: http://developer.eventbrite.com/
  baseURL: https://www.eventbriteapi.com//v3//series/{id}/events/
  tags: Series,,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/seriesidevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/seriesidevents-get-openapi.md
- name: Eventbrite Add Series  Events
  x-api-slug: eventbrite
  description: |-
    Creates more event dates or updates or deletes existing event dates in a repeating event series. In order for a series
    date to be deleted or updated, there must be no pending or completed orders for that date.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/eventbritelogoff8000gradient.png
  humanURL: http://developer.eventbrite.com/
  baseURL: https://www.eventbriteapi.com//v3//series/{id}/events/
  tags: Series,,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/seriesidevents-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/seriesidevents-post-openapi.md
- name: Eventbrite
  x-api-slug: eventbrite
  description: Eventbrite believes that anyone can be an event organizer. That&rsquo;s
    why they offer tools that make it easy to sell tickets to all kinds of events
    whether it&rsquo;s a photography class or a sold-out concert, an inspiring conference
    or an air-guitar competition. With Eventbrite, organizers can create a customizable
    event page; spread the word with social media; collect money; and gain visibility
    into attendees and sales. Eventbrite is for anyone planning or attending an event.
    It empowers event organizers to become more efficient and effective when bringing
    people together. And people everywhere are searching Eventbrite to discover great
    events that matter to them.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/eventbritelogoff8000gradient.png
  humanURL: http://developer.eventbrite.com/
  baseURL: https://www.eventbriteapi.com//v3
  tags: Series
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/series/master/_listings/eventbrite/openapi.md
x-common:
- type: x-apigee-console
  url: https://api.apigee.com/v1/consoles/eventbrite/apidescription?format=internal&ver=1351170233000
- type: x-authentication
  url: https://developer.eventbrite.com/docs/auth/
- type: x-base
  url: https://www.eventbriteapi.com/
- type: x-blog
  url: http://blog.eventbrite.com/
- type: x-blog-rss
  url: http://blog.eventbrite.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/eventbrite
- type: x-developer
  url: https://developer.eventbrite.com/
- type: x-github
  url: https://github.com/eventbrite
- type: x-pricing
  url: http://help.eventbrite.com/customer/en_us/portal/articles/428604
- type: x-privacy
  url: http://www.eventbrite.com/privacypolicy
- type: x-sdksio
  url: https://sdks.io/SDK/View/eventbrite
- type: x-selfservice-registration
  url: https://www.eventbrite.com/signup/?referrer=%2F%3Fshow_onboarding%3D1&user_type=prebuyer&user_type_sig=AH_ElWGNJ_zHaAxwjzt5jiCRmvPvNBsy6w
- type: x-terms-of-service
  url: http://www.eventbrite.com/tos
- type: x-twitter
  url: https://twitter.com/EventbriteAPI
- type: x-website
  url: http://developer.eventbrite.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---