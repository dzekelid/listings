---
name: Etsy
x-slug: etsy
description: Find handmade, vintage, and unique goods that express who you are.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
x-kinRank: "9"
x-alexaRank: "187"
tags: Listings
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/apis.md
specificationVersion: "0.14"
apis:
- name: Etsy Get Users User Favorites Listings
  x-api-slug: etsy
  description: Finds all favorite listings for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/favorites/listings
  tags: Users,Favorites,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/usersuser-idfavoriteslistings-get-openapi.md
- name: Etsy Get Users User Favorites Listings Listing
  x-api-slug: etsy
  description: Finds a favorite listing for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/favorites/listings/{listing_id}
  tags: Users,Favorites,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/usersuser-idfavoriteslistingslisting-id-get-openapi.md
- name: Etsy Post Users User Favorites Listings Listing
  x-api-slug: etsy
  description: Creates a new favorite listing for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/favorites/listings/{listing_id}
  tags: Users,Favorites,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/usersuser-idfavoriteslistingslisting-id-post-openapi.md
- name: Etsy Delete Users User Favorites Listings Listing
  x-api-slug: etsy
  description: Delete a favorite listing for a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/favorites/listings/{listing_id}
  tags: Users,Favorites,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/usersuser-idfavoriteslistingslisting-id-delete-openapi.md
- name: Etsy Get Homepages Pickers Featured Listing Picker Listings
  x-api-slug: etsy
  description: Retrieves a set of Listing objects associated to a FeaturedListingPicker.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///homepages/pickers/{featured_listing_picker_id}/listings
  tags: Home Pages,Pickers,Featured,Listing,Picker,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/homepagespickersfeatured-listing-picker-idlistings-get-openapi.md
- name: Etsy Get Homepages Pickers Featured Listing Picker Listings Active
  x-api-slug: etsy
  description: Retrieves a set of Listing objects associated to a FeaturedListingPicker
    in scope active.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///homepages/pickers/{featured_listing_picker_id}/listings/active
  tags: Home Pages,Pickers,Featured,Listing,Picker,Listings,Active
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/homepagespickersfeatured-listing-picker-idlistingsactive-get-openapi.md
- name: Etsy Get Homepages Listings
  x-api-slug: etsy
  description: Finds all FeaturedListings regardless of Listing state
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///homepages/listings/
  tags: Home Pages,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/homepageslistings-get-openapi.md
- name: Etsy Get Homepages Listings Active
  x-api-slug: etsy
  description: Finds all FeaturedListings that point to active Listings
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///homepages/listings/active
  tags: Home Pages,Listings,Active
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/homepageslistingsactive-get-openapi.md
- name: Etsy Get Homepages Listings Featured Listing
  x-api-slug: etsy
  description: Retrieves a FeaturedListing by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///homepages/listings/{featured_listing_id}
  tags: Home Pages,Listings,Featured,Listing
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/homepageslistingsfeatured-listing-id-get-openapi.md
- name: Etsy Get Homepages Listings Featured Listing Picker
  x-api-slug: etsy
  description: Retrieves a set of FeaturedListingPicker objects associated to a FeaturedListing.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///homepages/listings/{featured_listing_id}/picker
  tags: Home Pages,Listings,Featured,Listing,Picker
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/homepageslistingsfeatured-listing-idpicker-get-openapi.md
- name: Etsy Get Homepages Listings Featured Listing Listing
  x-api-slug: etsy
  description: Retrieves a set of Listing objects associated to a FeaturedListing.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///homepages/listings/{featured_listing_id}/listing
  tags: Home Pages,Listings,Featured,Listing,Listing
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/homepageslistingsfeatured-listing-idlisting-get-openapi.md
- name: Etsy Get Listings Listing Images Listing Image
  x-api-slug: etsy
  description: Retrieves a ListingImage by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///listings/{listing_id}/images/{listing_image_id}
  tags: Listings,Images,Listing,Image
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/listingslisting-idimageslisting-image-id-get-openapi.md
- name: Etsy Delete Listings Listing Images Listing Image
  x-api-slug: etsy
  description: Deletes a listing image
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///listings/{listing_id}/images/{listing_image_id}
  tags: Listings,Images,Listing,Image
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/listingslisting-idimageslisting-image-id-delete-openapi.md
- name: Etsy Post Listings Listing Images
  x-api-slug: etsy
  description: Upload a new listing image
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///listings/{listing_id}/images
  tags: Listings,Images
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/listingslisting-idimages-post-openapi.md
- name: Etsy Get Listings Listing Images
  x-api-slug: etsy
  description: Retrieves a set of ListingImage objects associated to a Listing.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///listings/{listing_id}/images
  tags: Listings,Images
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/listingslisting-idimages-get-openapi.md
- name: Etsy Get Listings Listing
  x-api-slug: etsy
  description: Retrieves a Listing by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///listings/{listing_id}
  tags: Listings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/listingslisting-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/listingslisting-id-get-openapi.md
- name: Etsy Put Listings Listing
  x-api-slug: etsy
  description: Updates a Listing
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///listings/{listing_id}
  tags: Listings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/listingslisting-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/listingslisting-id-put-openapi.md
- name: Etsy Delete Listings Listing
  x-api-slug: etsy
  description: Deletes a Listing
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///listings/{listing_id}
  tags: Listings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/listingslisting-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/listingslisting-id-delete-openapi.md
- name: Etsy Get Listings Listing Favored By
  x-api-slug: etsy
  description: Retrieves a set of FavoriteListing objects associated to a Listing.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///listings/{listing_id}/favored-by
  tags: Listings,Favored-by
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/listingslisting-idfavoredby-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/listingslisting-idfavoredby-get-openapi.md
- name: Etsy Get Listings Listing Shipping Info
  x-api-slug: etsy
  description: Retrieves a set of ShippingInfo objects associated to a Listing.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///listings/{listing_id}/shipping/info
  tags: Listings,Shipping,Info
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/listingslisting-idshippinginfo-get-openapi.md
- name: Etsy Post Listings Listing Shipping Info
  x-api-slug: etsy
  description: Creates a new ShippingInfo.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///listings/{listing_id}/shipping/info
  tags: Listings,Shipping,Info
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/listingslisting-idshippinginfo-post-openapi.md
- name: Etsy Get Listings Listing Payments
  x-api-slug: etsy
  description: Retrieves a set of ListingPayment objects associated to a Listing.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///listings/{listing_id}/payments
  tags: Listings,Payments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/listingslisting-idpayments-get-openapi.md
- name: Etsy Get Listings Active
  x-api-slug: etsy
  description: Finds all active Listing
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///listings/active
  tags: Listings,Active
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/listingsactive-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/listingsactive-get-openapi.md
- name: Etsy Get Shops Shop Listings Active
  x-api-slug: etsy
  description: Finds all active Listings associated with a Shop
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///shops/{shop_id}/listings/active
  tags: Shops,Shop,Listings,Active
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/shopsshop-idlistingsactive-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/shopsshop-idlistingsactive-get-openapi.md
- name: Etsy Post Listings
  x-api-slug: etsy
  description: Creates a new Listing
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///listings
  tags: Listings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/listings-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/listings-post-openapi.md
- name: Etsy Get Users User Recommended Listings
  x-api-slug: etsy
  description: Get recommended listings for an authenticated member. The number of
    listings returned may not match the specified limit if there is no activity from
    recommended shops.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/recommended_listings
  tags: Users,Recommended,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/usersuser-idrecommended-listings-get-openapi.md
- name: Etsy Post Users User Recommended Listings Rejects Listing S
  x-api-slug: etsy
  description: Registers rejections of recommended listings. Affects future recommended
    listings.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/recommended_listings/rejects/{listing_ids}
  tags: Users,Recommended,Listings,Rejects,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/usersuser-idrecommended-listingsrejectslisting-ids-post-openapi.md
- name: Etsy Post Users User Recommended Listings Views Listing S
  x-api-slug: etsy
  description: Register viewings of recommended listings. Affects future recommended
    listings.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/recommended_listings/views/{listing_ids}
  tags: Users,Recommended,Listings,Views,Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/usersuser-idrecommended-listingsviewslisting-ids-post-openapi.md
- name: Etsy Get Shops Shop Listings Featured
  x-api-slug: etsy
  description: Retrieves Listings associated to a Shop that are featured
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///shops/{shop_id}/listings/featured
  tags: Shops,Shop,Listings,Featured
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/shopsshop-idlistingsfeatured-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/shopsshop-idlistingsfeatured-get-openapi.md
- name: Etsy Get Shops Shop Listings Inactive
  x-api-slug: etsy
  description: Retrieves Listings associated to a Shop that are inactive
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///shops/{shop_id}/listings/inactive
  tags: Shops,Shop,Listings,Inactive
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/shopsshop-idlistingsinactive-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/shopsshop-idlistingsinactive-get-openapi.md
- name: Etsy Get Shops Shop Listings Expired
  x-api-slug: etsy
  description: Retrieves Listings associated to a Shop that are expired
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///shops/{shop_id}/listings/expired
  tags: Shops,Shop,Listings,Expired
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/shopsshop-idlistingsexpired-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/shopsshop-idlistingsexpired-get-openapi.md
- name: Etsy Get Shops Shop Listings Inactive Listing
  x-api-slug: etsy
  description: Retrieves a Listing associated to a Shop that is inactive
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///shops/{shop_id}/listings/inactive/{listing_id}
  tags: Shops,Shop,Listings,Inactive,Listing
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/shopsshop-idlistingsinactivelisting-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/shopsshop-idlistingsinactivelisting-id-get-openapi.md
- name: Etsy Get Shops Shop Listings Expired Listing
  x-api-slug: etsy
  description: Retrieves a Listing associated to a Shop that is inactive
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///shops/{shop_id}/listings/expired/{listing_id}
  tags: Shops,Shop,Listings,Expired,Listing
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/shopsshop-idlistingsexpiredlisting-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/shopsshop-idlistingsexpiredlisting-id-get-openapi.md
- name: Etsy
  x-api-slug: etsy
  description: Etsy is a handmade marketplace. The Etsy API lets developers tap into
    the Etsy community, building their own Etsy-powered applications for the web,
    desktop and mobile devices. Applications built on the API will connect buyers
    with sellers, promote the handmade lifestyle, and support the craftspeople who
    sell on Etsy.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private/
  tags: Listings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/listings/master/_listings/etsy/openapi.md
x-common:
- type: x-api-json--authoritative
  url: http://apis.io/apisdef/etsy.json
- type: x-application-gallery
  url: https://www.etsy.com/apps/
- type: x-base
  url: https://openapi.etsy.com/
- type: x-blog
  url: http://www.etsy.com/blog/en/
- type: x-blog-rss
  url: https://blog.etsy.com/en/feed/
- type: x-copyright
  url: https://www.etsy.com/help/article/482/?ref=ftr
- type: x-crunchbase
  url: https://crunchbase.com/organization/etsy
- type: x-crunchbase
  url: http://www.crunchbase.com/company/etsy
- type: x-developer
  url: https://www.etsy.com/developers/
- type: x-email
  url: enaffiliates@etsy.com
- type: x-email
  url: selleraffiliate@etsy.com
- type: x-email
  url: developer@etsy.com
- type: x-email
  url: legal@etsy.com
- type: x-email
  url: dpo@etsy.com
- type: x-email
  url: dispute-resolution@etsy.com
- type: x-forum
  url: https://www.etsy.com/developers/discussion
- type: x-github
  url: https://github.com/etsy
- type: x-privacy
  url: https://www.etsy.com/help/article/480/?ref=ftr
- type: x-terms-of-service
  url: https://www.etsy.com/help/article/479/?ref=ftr
- type: x-transparency-report
  url: http://blog.etsy.com/news/files/2015/07/Etsy_TransparencyReport_2014.pdf
- type: x-twitter
  url: https://twitter.com/Etsy
- type: x-website
  url: http://www.etsy.com/
- type: x-website
  url: http://etsy.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---