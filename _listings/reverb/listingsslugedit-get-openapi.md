---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 0
info:
  title: Reverb Get Listings Slug Edit
  description: Get listings slug edit.
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /comparison_shopping_pages/{id}/listings:
    get:
      summary: Get Comparison Shopping Pages Listings
      description: Return new or used listings for a comparison shopping page
      operationId: getComparisonShoppingPagesListings
      x-api-path-slug: comparison-shopping-pagesidlistings-get
      parameters:
      - in: query
        name: condition
        description: Condition of the listing
      - in: path
        name: id
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      responses:
        200:
          description: OK
      tags:
      - Comparison
      - Shopping
      - Pages
      - Id
      - Listings
  /listings:
    get:
      summary: Get Listings
      description: Default search of listings includes only used & handmade. Add a
        filter to view all listings or use the /listings/all endpoint.
      operationId: getListings
      x-api-path-slug: listings-get
      parameters:
      - in: query
        name: accepts_gift_cards
        description: If true, include only items that accept gift cards
      - in: query
        name: accepts_payment_plans
        description: If true, only show items that can be purchased with a payment
          plan
      - in: query
        name: auction_price_max
        description: Maximum current auction price
      - in: query
        name: category
        description: Category slug from /api/categories
      - in: query
        name: conditions
        description: 'Condition: all,new,b-stock,used,non-functioning'
      - in: query
        name: currency
        description: The currency to be used for the price filters
      - in: query
        name: decade
        description: 'Decade: e'
      - in: query
        name: exclude_auctions
        description: If true, exclude auctions
      - in: query
        name: finish
        description: Visual finish of the item, common for guitars
      - in: query
        name: handmade
        description: Handmade items only
      - in: query
        name: item_city
        description: City where item is located
      - in: query
        name: item_country
        description: DEPRECATED - Country code where item is located
      - in: query
        name: item_region
        description: Country code where item is located
      - in: query
        name: item_state
        description: State or region code where item is located
      - in: query
        name: listing_type
        description: 'Type of listing: auctions,offers'
      - in: query
        name: make
        description: Make(s)/brand of item (e
      - in: query
        name: model
        description: Model of item (e
      - in: query
        name: must_not
        description: Search term negation
      - in: query
        name: not_ids
        description: Listing ID negation
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: preferred_seller
        description: If true, include only items by Reverb Preferred Sellers
      - in: query
        name: price_max
        description: Maximum price of search results (USD)
      - in: query
        name: price_min
        description: Minimum price of search results (USD)
      - in: query
        name: product_type
        description: Product type slug from /api/categories
      - in: query
        name: query
        description: Search query
      - in: query
        name: ships_to
        description: Limit search to items that ship to this country code
      - in: query
        name: shop
        description: Slug of shop to search
      - in: query
        name: shop_id
        description: ID of shop to search
      - in: query
        name: watchers_count_min
        description: Minimum number of watchers (used to find popular items)
      - in: query
        name: year_max
        description: Maximum year of manufacture
      - in: query
        name: year_min
        description: Minumum year of manufacture
      responses:
        200:
          description: OK
      tags:
      - Listings
    post:
      summary: Post Listings
      description: Create a listing
      operationId: postListings
      x-api-path-slug: listings-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Listings
  /listings/all:
    get:
      summary: Get Listings All
      description: All listings including used, handmade, and brand new
      operationId: getListingsAll
      x-api-path-slug: listingsall-get
      parameters:
      - in: query
        name: accepts_gift_cards
        description: If true, include only items that accept gift cards
      - in: query
        name: accepts_payment_plans
        description: If true, only show items that can be purchased with a payment
          plan
      - in: query
        name: auction_price_max
        description: Maximum current auction price
      - in: query
        name: category
        description: Category slug from /api/categories
      - in: query
        name: conditions
        description: 'Condition: all,new,b-stock,used,non-functioning'
      - in: query
        name: currency
        description: The currency to be used for the price filters
      - in: query
        name: decade
        description: 'Decade: e'
      - in: query
        name: exclude_auctions
        description: If true, exclude auctions
      - in: query
        name: finish
        description: Visual finish of the item, common for guitars
      - in: query
        name: handmade
        description: Handmade items only
      - in: query
        name: item_city
        description: City where item is located
      - in: query
        name: item_country
        description: DEPRECATED - Country code where item is located
      - in: query
        name: item_region
        description: Country code where item is located
      - in: query
        name: item_state
        description: State or region code where item is located
      - in: query
        name: listing_type
        description: 'Type of listing: auctions,offers'
      - in: query
        name: make
        description: Make(s)/brand of item (e
      - in: query
        name: model
        description: Model of item (e
      - in: query
        name: must_not
        description: Search term negation
      - in: query
        name: not_ids
        description: Listing ID negation
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: preferred_seller
        description: If true, include only items by Reverb Preferred Sellers
      - in: query
        name: price_max
        description: Maximum price of search results (USD)
      - in: query
        name: price_min
        description: Minimum price of search results (USD)
      - in: query
        name: product_type
        description: Product type slug from /api/categories
      - in: query
        name: query
        description: Search query
      - in: query
        name: ships_to
        description: Limit search to items that ship to this country code
      - in: query
        name: shop
        description: Slug of shop to search
      - in: query
        name: shop_id
        description: ID of shop to search
      - in: query
        name: watchers_count_min
        description: Minimum number of watchers (used to find popular items)
      - in: query
        name: year_max
        description: Maximum year of manufacture
      - in: query
        name: year_min
        description: Minumum year of manufacture
      responses:
        200:
          description: OK
      tags:
      - Listings
  /listings/facets/seller_location:
    get:
      summary: Get Listings Facets Seller Location
      description: Get listings facets seller location.
      operationId: getListingsFacetsSellerLocation
      x-api-path-slug: listingsfacetsseller-location-get
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Facets
      - Seller
      - Location
  /listings/{id}/negotiation:
    get:
      summary: Get Listings Negotiation
      description: Returns the latest negotiation for the requesting user given a
        listing id
      operationId: getListingsNegotiation
      x-api-path-slug: listingsidnegotiation-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Id
      - Negotiation
  /listings/{id}/offer:
    post:
      summary: Post Listings Offer
      description: Make an offer to the seller of a listing
      operationId: postListingsOffer
      x-api-path-slug: listingsidoffer-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Id
      - Offer
  /listings/{listing_id}/bump:
    get:
      summary: Get Listings Listing Bump
      description: View available bump tiers and stats for a listing
      operationId: getListingsListingBump
      x-api-path-slug: listingslisting-idbump-get
      parameters:
      - in: path
        name: listing_id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Listing
      - Id
      - Bump
  /listings/{listing_id}/bump/{budget_type}:
    post:
      summary: Post Listings Listing Bump Budget Type
      description: Post listings listing bump budget type.
      operationId: postListingsListingBumpBudgetType
      x-api-path-slug: listingslisting-idbumpbudget-type-post
      parameters:
      - in: path
        name: budget_type
      - in: path
        name: listing_id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Listing
      - Id
      - Bump
      - Budget
      - Type
  /listings/{listing_id}/conversations:
    post:
      summary: Post Listings Listing Conversations
      description: Post listings listing conversations.
      operationId: postListingsListingConversations
      x-api-path-slug: listingslisting-idconversations-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: listing_id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Listing
      - Id
      - Conversations
  /listings/{listing_id}/images:
    get:
      summary: Get Listings Listing Images
      description: View the images associated with a particular listing
      operationId: getListingsListingImages
      x-api-path-slug: listingslisting-idimages-get
      parameters:
      - in: path
        name: listing_id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Listing
      - Id
      - Images
  /listings/{listing_id}/images/{image_id}:
    delete:
      summary: Delete Listings Listing Images Image
      description: Delete listings listing images image.
      operationId: deleteListingsListingImagesImage
      x-api-path-slug: listingslisting-idimagesimage-id-delete
      parameters:
      - in: path
        name: image_id
      - in: path
        name: listing_id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Listing
      - Id
      - Images
      - Image
      - Id
  /listings/{listing_id}/product_bundle:
    get:
      summary: Get Listings Listing Product Bundle
      description: Find a product bundle attached to a listing
      operationId: getListingsListingProductBundle
      x-api-path-slug: listingslisting-idproduct-bundle-get
      parameters:
      - in: query
        name: for_seller
        description: Pass to see non-live bundles as the seller
      - in: path
        name: listing_id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Listing
      - Id
      - Product
      - Bundle
  /listings/{listing_id}/sales:
    get:
      summary: Get Listings Listing Sales
      description: See all sales that include a listing.
      operationId: getListingsListingSales
      x-api-path-slug: listingslisting-idsales-get
      parameters:
      - in: path
        name: listing_id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Listing
      - Id
      - Sales
  /listings/{slug}:
    delete:
      summary: Delete Listings Slug
      description: Delete a draft listing. Cannot be used on non-drafts.
      operationId: deleteListingsSlug
      x-api-path-slug: listingsslug-delete
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
    get:
      summary: Get Listings Slug
      description: Get listings slug.
      operationId: getListingsSlug
      x-api-path-slug: listingsslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
    put:
      summary: Put Listings Slug
      description: Put listings slug.
      operationId: putListingsSlug
      x-api-path-slug: listingsslug-put
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
  /listings/{slug}/edit:
    get:
      summary: Get Listings Slug Edit
      description: Get listings slug edit.
      operationId: getListingsSlugEdit
      x-api-path-slug: listingsslugedit-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
      - Edit
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---