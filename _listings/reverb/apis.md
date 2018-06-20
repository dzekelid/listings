---
name: Reverb
x-slug: reverb
description: 'Reverb&#8217;s mission is to connect people with meaningful content.Reverb
  was created to find and connect the rich associations between words, ideas, content,
  and people. Through our products, we enhance broader knowledge around favorite topics
  by surfacing interesting information readers might not uncover on their own. We
  make tools for content understanding at every level from the single word on up.
  Wordnik: Get a full view of any word you???re interested in, with definitions, example
  sentences, related words, tweets from Twitter, pictures from Flickr, and much more.Reverb
  for Publishers: Reverb for Publishers brings relevant content to web audiences and
  surfaces additional content for publishers.Reverb for Developers: Reverb is committed
  to the open-source community and is proudly contributing infrastructure software
  to power applications and enterprises both small and gigantic. Our involvement with
  the Wordnik API, Scalatra, Swagger and Atmosphere is detailed on our site.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Listings
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/apis.md
specificationVersion: "0.14"
apis:
- name: reverb Get Comparison Shopping Pages Listings
  x-api-slug: reverb
  description: Return new or used listings for a comparison shopping page
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//comparison_shopping_pages/{id}/listings
  tags: Comparison,Shopping,Pages,Id,Listings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/comparison-shopping-pagesidlistings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/comparison-shopping-pagesidlistings-get-openapi.md
- name: reverb Get Listings
  x-api-slug: reverb
  description: Default search of listings includes only used & handmade. Add a filter
    to view all listings or use the /listings/all endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings
  tags: Listings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listings-get-openapi.md
- name: reverb Post Listings
  x-api-slug: reverb
  description: Create a listing
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings
  tags: Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listings-post-openapi.md
- name: reverb Get Listings All
  x-api-slug: reverb
  description: All listings including used, handmade, and brand new
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/all
  tags: Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingsall-get-openapi.md
- name: reverb Get Listings Facets Seller Location
  x-api-slug: reverb
  description: Get listings facets seller location.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/facets/seller_location
  tags: Listings,Facets,Seller,Location
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingsfacetsseller-location-get-openapi.md
- name: reverb Get Listings Negotiation
  x-api-slug: reverb
  description: Returns the latest negotiation for the requesting user given a listing
    id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/{id}/negotiation
  tags: Listings,Id,Negotiation
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingsidnegotiation-get-openapi.md
- name: reverb Post Listings Offer
  x-api-slug: reverb
  description: Make an offer to the seller of a listing
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/{id}/offer
  tags: Listings,Id,Offer
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingsidoffer-post-openapi.md
- name: reverb Get Listings Listing Bump
  x-api-slug: reverb
  description: View available bump tiers and stats for a listing
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/{listing_id}/bump
  tags: Listings,Listing,Id,Bump
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingslisting-idbump-get-openapi.md
- name: reverb Post Listings Listing Bump Budget Type
  x-api-slug: reverb
  description: Post listings listing bump budget type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/{listing_id}/bump/{budget_type}
  tags: Listings,Listing,Id,Bump,Budget,Type
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingslisting-idbumpbudget-type-post-openapi.md
- name: reverb Post Listings Listing Conversations
  x-api-slug: reverb
  description: Post listings listing conversations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/{listing_id}/conversations
  tags: Listings,Listing,Id,Conversations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingslisting-idconversations-post-openapi.md
- name: reverb Get Listings Listing Images
  x-api-slug: reverb
  description: View the images associated with a particular listing
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/{listing_id}/images
  tags: Listings,Listing,Id,Images
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingslisting-idimages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingslisting-idimages-get-openapi.md
- name: reverb Delete Listings Listing Images Image
  x-api-slug: reverb
  description: Delete listings listing images image.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/{listing_id}/images/{image_id}
  tags: Listings,Listing,Id,Images,Image,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingslisting-idimagesimage-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingslisting-idimagesimage-id-delete-openapi.md
- name: reverb Get Listings Listing Product Bundle
  x-api-slug: reverb
  description: Find a product bundle attached to a listing
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/{listing_id}/product_bundle
  tags: Listings,Listing,Id,Product,Bundle
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingslisting-idproduct-bundle-get-openapi.md
- name: reverb Get Listings Listing Sales
  x-api-slug: reverb
  description: See all sales that include a listing.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/{listing_id}/sales
  tags: Listings,Listing,Id,Sales
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingslisting-idsales-get-openapi.md
- name: reverb Delete Listings Slug
  x-api-slug: reverb
  description: Delete a draft listing. Cannot be used on non-drafts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/{slug}
  tags: Listings,Slug
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingsslug-delete-openapi.md
- name: reverb Get Listings Slug
  x-api-slug: reverb
  description: Get listings slug.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/{slug}
  tags: Listings,Slug
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingsslug-get-openapi.md
- name: reverb Put Listings Slug
  x-api-slug: reverb
  description: Put listings slug.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/{slug}
  tags: Listings,Slug
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingsslug-put-openapi.md
- name: reverb Get Listings Slug Edit
  x-api-slug: reverb
  description: Get listings slug edit.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/{slug}/edit
  tags: Listings,Slug,Edit
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingsslugedit-get-openapi.md
- name: reverb Post Listings Slug Flag
  x-api-slug: reverb
  description: Flag a listing for inappropriate content or fraud
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/{slug}/flag
  tags: Listings,Slug,Flag
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingsslugflag-post-openapi.md
- name: reverb Get Listings Slug Reviews
  x-api-slug: reverb
  description: Get listings slug reviews.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/{slug}/reviews
  tags: Listings,Slug,Reviews
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingsslugreviews-get-openapi.md
- name: reverb Post Listings Slug Reviews
  x-api-slug: reverb
  description: Create a review for a listing
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/{slug}/reviews
  tags: Listings,Slug,Reviews
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingsslugreviews-post-openapi.md
- name: reverb Get Listings Slug Similar Listings
  x-api-slug: reverb
  description: Get listings slug similar listings.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/{slug}/similar_listings
  tags: Listings,Slug,Similar,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/listingsslugsimilar-listings-get-openapi.md
- name: reverb Get My Listings
  x-api-slug: reverb
  description: Retrieve a list of live listings for the seller. To search all listings
    specify state=all
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/listings
  tags: My,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/mylistings-get-openapi.md
- name: reverb Get My Listings Drafts
  x-api-slug: reverb
  description: Retrieve a list your draft listings
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/listings/drafts
  tags: My,Listings,Drafts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/mylistingsdrafts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/mylistingsdrafts-get-openapi.md
- name: reverb Get My Listings Negotiations
  x-api-slug: reverb
  description: Get a list of active negotiations as a seller
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/listings/negotiations
  tags: My,Listings,Negotiations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/mylistingsnegotiations-get-openapi.md
- name: reverb Put My Listings Slug State End
  x-api-slug: reverb
  description: Put my listings slug state end.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/listings/{slug}/state/end
  tags: My,Listings,Slug,State,End
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/mylistingsslugstateend-put-openapi.md
- name: reverb Get My Viewed Listings
  x-api-slug: reverb
  description: Get a list of your recently viewed listings.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/viewed_listings
  tags: My,Viewed,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/myviewed-listings-get-openapi.md
- name: reverb Delete Sales Sale Listings
  x-api-slug: reverb
  description: Remove a listing from a sale
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//sales/{sale_id}/listings
  tags: Sales,Sale,Id,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/salessale-idlistings-delete-openapi.md
- name: reverb Post Sales Sale Listings
  x-api-slug: reverb
  description: Post sales sale listings.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//sales/{sale_id}/listings
  tags: Sales,Sale,Id,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/salessale-idlistings-post-openapi.md
- name: reverb Get Articles Slug Related Listings
  x-api-slug: reverb
  description: Find listings related to an article
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//articles/{slug}/related-listings
  tags: Articles,Slug,Related-listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/articlesslugrelatedlistings-get-openapi.md
- name: reverb Get Vinyl Listings
  x-api-slug: reverb
  description: Get vinyl listings.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//vinyl/listings
  tags: Vinyl,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/vinyllistings-get-openapi.md
- name: reverb Post Vinyl Listings
  x-api-slug: reverb
  description: Post vinyl listings.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//vinyl/listings
  tags: Vinyl,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/vinyllistings-post-openapi.md
- name: reverb Get Vinyl Listings
  x-api-slug: reverb
  description: Get vinyl listings.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//vinyl/listings/{id}
  tags: Vinyl,Listings,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/vinyllistingsid-get-openapi.md
- name: reverb
  x-api-slug: reverb
  description: 'Reverb&#8217;s mission is to connect people with meaningful content.Reverb
    was created to find and connect the rich associations between words, ideas, content,
    and people. Through our products, we enhance broader knowledge around favorite
    topics by surfacing interesting information readers might not uncover on their
    own. We make tools for content understanding at every level from the single word
    on up. Wordnik: Get a full view of any word you???re interested in, with definitions,
    example sentences, related words, tweets from Twitter, pictures from Flickr, and
    much more.Reverb for Publishers: Reverb for Publishers brings relevant content
    to web audiences and surfaces additional content for publishers.Reverb for Developers:
    Reverb is committed to the open-source community and is proudly contributing infrastructure
    software to power applications and enterprises both small and gigantic. Our involvement
    with the Wordnik API, Scalatra, Swagger and Atmosphere is detailed on our site.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api
  tags: Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/reverb/openapi.md
x-common:
- type: x-blog
  url: http://blog.helloreverb.com/
- type: x-blog-rss
  url: http://blog.helloreverb.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/reverb-technologies
- type: x-github
  url: https://github.com/reverb
- type: x-twitter
  url: https://twitter.com/reverb
- type: x-website
  url: https://helloreverb.com/app
- type: x-website
  url: http://reverb.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---