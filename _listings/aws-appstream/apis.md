---
name: AWS AppStream
x-slug: aws-appstream
description: Amazon AppStream is a fully managed, secure application streaming service
  that allows you to stream desktop applications from AWS to any device running a
  web browser, without rewriting them. Amazon AppStream 2.0 provides users instant-on
  access to the applications they need, and a responsive, fluid user experience on
  the device of their choice.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/appstream2_try_it_now_2_big.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Associated
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/associated/master/_listings/aws-appstream/apis.md
specificationVersion: "0.14"
apis:
- name: AWS AppStream 2.0 API - List Associated Fleets
  x-api-slug: actionlistassociatedfleets-get
  description: Lists all fleets associated with the stack.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/appstream2_try_it_now_2_big.png
  humanURL: https://aws.amazon.com/appstream2/
  baseURL: :///
  tags: Amazon Web Services, Applications, Stack Network, API Service Provider, API
    Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/associated/master/_listings/aws-appstream/actionlistassociatedfleets-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/associated/master/_listings/aws-appstream/actionlistassociatedfleets-get-openapi.md
- name: AWS AppStream 2.0 API - List Associated Stacks
  x-api-slug: actionlistassociatedstacks-get
  description: Lists all stacks to which the specified fleet is associated.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/appstream2_try_it_now_2_big.png
  humanURL: https://aws.amazon.com/appstream2/
  baseURL: :///
  tags: Amazon Web Services, Applications, Stack Network, API Service Provider, API
    Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/associated/master/_listings/aws-appstream/actionlistassociatedstacks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/associated/master/_listings/aws-appstream/actionlistassociatedstacks-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.api.gateway.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.appstream.stack.network
- type: x-documentation
  url: http://docs.aws.amazon.com/appstream2/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/appstream2/faqs/
- type: x-forum
  url: https://aws.amazon.com/appstream2/resources/#forum
- type: x-getting-started
  url: https://aws.amazon.com/appstream2/resources/#getting_starte
- type: x-pricing
  url: https://aws.amazon.com/appstream2/pricing/
- type: x-website
  url: https://aws.amazon.com/appstream2/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---