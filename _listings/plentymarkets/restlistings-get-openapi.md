---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List listing
  description: Lists listings by filter options.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/listings:
    get:
      summary: List listing
      description: Lists listings by filter options.
      operationId: getRestListings
      x-api-path-slug: restlistings-get
      parameters:
      - in: query
        name: id
        description: Filter that restricts the search result to listings with specific
          listing ID
      - in: query
        name: itemId
        description: Filter that restricts the search result to listings with specific
          item ID
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: stockDependenceTypeId
        description: Filter that restricts the search result to listings with specific
          stock dependence type ID
      - in: query
        name: typeId
        description: Filter that restricts the search result to listings with specific
          type ID
      - in: query
        name: unitCombinationId
        description: Filter that restricts the search result to listings with specific
          unit combination ID
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
    post:
      summary: Create new listing
      description: Creates a new listing.
      operationId: postRestListings
      x-api-path-slug: restlistings-post
      parameters:
      - in: body
        name: /rest/listings
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Listing
  /rest/listings/markets:
    get:
      summary: List listing markets
      description: Lists listing market by filter options.
      operationId: getRestListingsMarkets
      x-api-path-slug: restlistingsmarkets-get
      parameters:
      - in: query
        name: credentialsId
        description: Filter that restricts the search result to listing markets with
          given credential ID
      - in: query
        name: directoryId
        description: Filter that restricts the search result to listing markets with
          a given directory ID
      - in: query
        name: duration
        description: Filter that restricts the search result to listing markets with
          given duration
      - in: query
        name: id
        description: Filter that restricts the search result to listing markets that
          match the given ID(s)
      - in: query
        name: itemId
        description: Filter that restricts the search result to listing markets that
          belong to a given item ID
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: listingId
        description: Filter that restricts the search result to listing markets that
          belong to a given listing ID
      - in: query
        name: listingTypeId
        description: Filter that restricts the search result to listing markets that
          belong to a listing of a custom type ID
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referrerId
        description: Filter that restricts the search result to listing markets with
          given referrer ID
      - in: query
        name: shippingProfileId
        description: Filter that restricts the search result to listing markets that
          belong to a given shipping profile ID
      - in: query
        name: status
        description: Filter that restricts the search result to listing markets with
          a custom status condition
      - in: query
        name: stockCondition
        description: Filter that restricts the search result to listing markets with
          a custom stock condition
      - in: query
        name: stockDependenceTypeId
        description: Filter that restricts the search result to listing markets that
          belong to a listing with a custom stock dependence type ID
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to listing markets that
          were last updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to listing markets that
          were last updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to listing markets that
          match the given variation ID(s)
      - in: query
        name: variations
        description: Filter that restricts the search result to listing markets with
          a custom variation condition
      - in: query
        name: verified
        description: Filter that restricts the search result to listing markets that
          are verified
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Markets
    post:
      summary: Create new listing market
      description: |-
        Creates a new listing market. Based on the given options this call can create multiple listing markets. If the
        'optionTemplateId' parameter is provided and the listing option template includes options for different markets
        than one listing market will be created for each market.
      operationId: postRestListingsMarkets
      x-api-path-slug: restlistingsmarkets-post
      parameters:
      - in: body
        name: /rest/listings/markets
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Listing
      - Market
  /rest/listings/markets/directories:
    get:
      summary: Get all listing market directories
      description: Gets all listing market directories.
      operationId: getRestListingsMarketsDirectories
      x-api-path-slug: restlistingsmarketsdirectories-get
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Directories
    post:
      summary: Create listing market directory
      description: Creates a listing market directory.
      operationId: postRestListingsMarketsDirectories
      x-api-path-slug: restlistingsmarketsdirectories-post
      parameters:
      - in: body
        name: /rest/listings/markets/directories
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Directory
  /rest/listings/markets/directories/{id}:
    delete:
      summary: Delete listing market directory
      description: Deletes a listing market directory by ID.
      operationId: deleteRestListingsMarketsDirectories
      x-api-path-slug: restlistingsmarketsdirectoriesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Directory
    get:
      summary: Get a listing market directory
      description: Gets a listing market directory by ID.
      operationId: getRestListingsMarketsDirectories
      x-api-path-slug: restlistingsmarketsdirectoriesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Directory
    put:
      summary: Update listing market directory
      description: Updates a listing market directory by ID.
      operationId: putRestListingsMarketsDirectories
      x-api-path-slug: restlistingsmarketsdirectoriesid-put
      parameters:
      - in: body
        name: /rest/listings/markets/directories/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Directory
  /rest/listings/markets/find:
    get:
      summary: Find listing markets
      description: Lists listing market by filter options.
      operationId: getRestListingsMarketsFind
      x-api-path-slug: restlistingsmarketsfind-get
      parameters:
      - in: query
        name: credentialsId
        description: Filter that restricts the search result to listing markets with
          given credential ID
      - in: query
        name: directoryId
        description: Filter that restricts the search result to listing markets with
          a given directory ID
      - in: query
        name: id
        description: Filter that restricts the search result to listing markets that
          match the given ID(s)
      - in: query
        name: itemId
        description: Filter that restricts the search result to listing markets that
          belong to a given item ID
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referrerId
        description: Filter that restricts the search result to listing markets with
          given referrer ID
      - in: query
        name: shippingProfileId
        description: Filter that restricts the search result to listing markets that
          belong to a given shipping profile ID
      - in: query
        name: variations
        description: Filter that restricts the search result to listing markets with
          a custom variation condition
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Find
      - Listing
      - Markets
  /rest/listings/markets/histories:
    get:
      summary: List listing market history
      description: Lists listing market history by filter options.
      operationId: getRestListingsMarketsHistories
      x-api-path-slug: restlistingsmarketshistories-get
      parameters:
      - in: query
        name: credentialsId
        description: Filter that restricts the search result to listing market histories
          with given credential ID
      - in: query
        name: directoryId
        description: Filter that restricts the search result to listing market histories
          with a given directory ID
      - in: query
        name: duration
        description: Filter that restricts the search result to listing market histories
          with given duration
      - in: query
        name: externalId
        description: Filter that restricts the search result to listing market histories
          with given external id
      - in: query
        name: firstPlatformCategoryId
        description: Filter that restricts the search result to listing market histories
          with first platform category ID equal to the given ID
      - in: query
        name: firstShopCategoryId
        description: Filter that restricts the search result to listing market histories
          with first shop category ID equal to the given ID
      - in: query
        name: isClickAndCollect
        description: Filter that restricts the search result to listing market histories
          that belong to eBay Click & Collect
      - in: query
        name: isEbayPlus
        description: Filter that restricts the search result to listing market histories
          that belong to eBay Plus
      - in: query
        name: itemId
        description: Filter that restricts the search result to listing market histories
          that belong to a given item ID
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: lastSale
        description: Filter that restricts the search result to listing market histories
          with last sale before given date
      - in: query
        name: listingId
        description: Filter that restricts the search result to listing market histories
          that belong to a given listing ID
      - in: query
        name: listingMarketId
        description: Filter that restricts the search result to listing market histories
          that match the given listing market ID(s)
      - in: query
        name: listingTypeId
        description: Filter that restricts the search result to listing market histories
          that belong to a listing of a custom type ID
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referrerId
        description: Filter that restricts the search result to listing market histories
          with given referrer ID
      - in: query
        name: secondPlatformCategoryId
        description: Filter that restricts the search result to listing market histories
          with second platform category ID equal to the given ID
      - in: query
        name: secondShopCategoryId
        description: Filter that restricts the search result to listing market histories
          with second shop category ID equal to the given ID
      - in: query
        name: shippingProfileId
        description: Filter that restricts the search result to listing market histories
          that belong to a given shipping profile
      - in: query
        name: statusId
        description: Filter that restricts the search result to listing market histories
          with a custom status status ID
      - in: query
        name: stockCondition
        description: Filter that restricts the search result to listing market histories
          with a custom stock condition
      - in: query
        name: stockDependenceTypeId
        description: Filter that restricts the search result to listing market histories
          that belong to a listing with a custom stock dependence type ID
      - in: query
        name: textData
        description: Filter that restricts the search result to listing market histories
          that match given text in listing title or description
      - in: query
        name: thirdShopCategoryId
        description: Filter that restricts the search result to listing market histories
          with third shop category ID equal to the given ID
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to listing market histories
          that were last updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to listing market histories
          that were last updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to listing market histories
          that match the given variation ID(s)
      - in: query
        name: variations
        description: Filter that restricts the search result to listing market histories
          with a custom variation condition
      - in: query
        name: verified
        description: Filter that restricts the search result to listing market histories
          that are verified
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Market
      - History
  /rest/listings/markets/histories/end/{id?}:
    delete:
      summary: End the listing
      description: Ends the listing on the designated market.
      operationId: deleteRestListingsMarketsHistoriesEnd
      x-api-path-slug: restlistingsmarketshistoriesendid-delete
      parameters:
      - in: query
        name: deleteOnSuccess
        description: Tells if the listing market history should also be deleted from
          the database
      - in: query
        name: id
        description: The ID of the listing market history that needs to be ended
      - in: path
        name: id?
      responses:
        200:
          description: OK
      tags:
      - End
      - Listing
  /rest/listings/markets/histories/relist/{id?}:
    post:
      summary: Relist the listing
      description: Relists the listing on the designated market.
      operationId: postRestListingsMarketsHistoriesRelist
      x-api-path-slug: restlistingsmarketshistoriesrelistid-post
      parameters:
      - in: query
        name: id
        description: The ID of the listing market history that needs to be relisted
      - in: path
        name: id?
      responses:
        200:
          description: OK
      tags:
      - Relist
      - Listing
  /rest/listings/markets/histories/update/{id?}:
    put:
      summary: Update listing market histories
      description: |-
        Updates listing market histories by given update options. The listing market histories are not directly revised,
        they are added to the batch processing lists, waiting to be revised by automated background processes.
      operationId: putRestListingsMarketsHistoriesUpdate
      x-api-path-slug: restlistingsmarketshistoriesupdateid-put
      parameters:
      - in: query
        name: id
        description: The ID of the listing market history that needs to be ended
      - in: path
        name: id?
      - in: query
        name: options
        description: Multiple update options
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Histories
  /rest/listings/markets/histories/{id}:
    get:
      summary: Get a listing market history
      description: Gets a listing market history by given ID.
      operationId: getRestListingsMarketsHistories
      x-api-path-slug: restlistingsmarketshistoriesid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - History
  /rest/listings/markets/infos:
    get:
      summary: Search listing market info
      description: Search listing market info by filter options.
      operationId: getRestListingsMarketsInfos
      x-api-path-slug: restlistingsmarketsinfos-get
      parameters:
      - in: query
        name: code
        description: Filter that restricts the search result to listing market info
          with given codes
      - in: query
        name: createdAtFrom
        description: Filter that restricts the search result to listing markets that
          were last updated on the specified date
      - in: query
        name: createdAtTo
        description: Filter that restricts the search result to listing markets that
          were last updated within a specified period of time
      - in: query
        name: id
        description: Filter that restricts the search result to listing market info
          that match the given ID(s)
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: listingMarketId
        description: Filter that restricts the search result to listing market info
          that match the given listing market ID(s)
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: type
        description: Filter that restricts the search result to listing market info
          with a custom type
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Search
      - Listing
      - Market
      - Info
  /rest/listings/markets/start/{id?}:
    post:
      summary: Start the market listing on the designated market.
      description: Starts the market listing on the designated markets.
      operationId: postRestListingsMarketsStart
      x-api-path-slug: restlistingsmarketsstartid-post
      parameters:
      - in: query
        name: distribution
        description: The number of minutes that the listing should be started
      - in: query
        name: id
        description: The ID of the listing market that needs to be started
      - in: path
        name: id?
      - in: query
        name: startAt
        description: When should the listings be started
      responses:
        200:
          description: OK
      tags:
      - Start
      - Market
      - Listing
      - "On"
      - Designated
      - Market
  /rest/listings/markets/texts:
    get:
      summary: List listing market texts
      description: Lists listing market texts by filter options.
      operationId: getRestListingsMarketsTexts
      x-api-path-slug: restlistingsmarketstexts-get
      parameters:
      - in: query
        name: contains
        description: Filter that restricts the search result to listing market texts
          which title, subtitle or description contain the given value
      - in: query
        name: id
        description: Filter that restricts the search result to listing market texts
          with specific ID
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: language
        description: Filter that restricts the search result to listing market texts
          for a specific language
      - in: query
        name: listingMarketId
        description: Filter that restricts the search result to listing market texts
          with specific listing market IDs
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Market
      - Texts
    post:
      summary: Create a listing market text
      description: Creates a listing market text for a given listing market ID. If
        an entry with same data already exists the request will be ignored and the
        old entry will be returned.
      operationId: postRestListingsMarketsTexts
      x-api-path-slug: restlistingsmarketstexts-post
      parameters:
      - in: body
        name: /rest/listings/markets/texts
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: listingMarketId
        description: The listing market ID this text belongs to
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Text
  /rest/listings/markets/texts/{id}:
    delete:
      summary: Delete a listing market text
      description: Deletes a listing market text for a given listing market text ID.
      operationId: deleteRestListingsMarketsTexts
      x-api-path-slug: restlistingsmarketstextsid-delete
      parameters:
      - in: path
        name: id
      - in: query
        name: lang
        description: The listing market text language that should be updated
      - in: query
        name: listingMarketId
        description: The listing market ID this text belongs to
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Text
    get:
      summary: Get a listing market text
      description: Gets a listing market text by providing its ID.
      operationId: getRestListingsMarketsTexts
      x-api-path-slug: restlistingsmarketstextsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Text
  /rest/listings/markets/texts/{listingMarketId}/{lang}:
    put:
      summary: Update a listing market text
      description: Updates a listing market text for a given listing market ID and
        language.
      operationId: putRestListingsMarketsTextsListingmarketLang
      x-api-path-slug: restlistingsmarketstextslistingmarketidlang-put
      parameters:
      - in: body
        name: /rest/listings/markets/texts/{listingMarketId}/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lang
      - in: path
        name: listingMarketId
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Text
  /rest/listings/markets/verify/{id?}:
    post:
      summary: Verify listing markets
      description: Verifies the listing markets.
      operationId: postRestListingsMarketsVerify
      x-api-path-slug: restlistingsmarketsverifyid-post
      parameters:
      - in: query
        name: id
        description: The ID of the listing market that need to be verified
      - in: path
        name: id?
      responses:
        200:
          description: OK
      tags:
      - Verify
      - Listing
      - Markets
  /rest/listings/markets/{id}:
    delete:
      summary: Delete listing market
      description: Deletes a listing market by ID.
      operationId: deleteRestListingsMarkets
      x-api-path-slug: restlistingsmarketsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
    get:
      summary: Get a listing market
      description: Gets a listing market by given ID.
      operationId: getRestListingsMarkets
      x-api-path-slug: restlistingsmarketsid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
    put:
      summary: Update a listing market
      description: Updates a listing market by ID.
      operationId: putRestListingsMarkets
      x-api-path-slug: restlistingsmarketsid-put
      parameters:
      - in: body
        name: /rest/listings/markets/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: query
        name: referrerId
        description: The referrer ID
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
  /rest/listings/shipping_profiles:
    get:
      summary: List listing shipping profiles
      description: Lists listing shipping profiles.
      operationId: getRestListingsShippingProfiles
      x-api-path-slug: restlistingsshipping-profiles-get
      parameters:
      - in: query
        name: credentialsId
        description: Filter that restricts the search result to listing shipping profiles
          with given credential ID(s)
      - in: query
        name: id
        description: Filter that restricts the search result to listing shipping profiles
          that match the given ID(s)
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referrerId
        description: Filter that restricts the search result to listing shipping profiles
          with given referrer ID(s)
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Shipping
      - Profiles
  /rest/listings/stock_dependence_types:
    get:
      summary: List listing stock dependence types
      description: Lists listing stock dependence types.
      operationId: getRestListingsStockDependenceTypes
      x-api-path-slug: restlistingsstock-dependence-types-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Stock
      - Dependence
      - Types
  /rest/listings/stock_dependence_types/{id}:
    get:
      summary: Get a listing stock dependence type
      description: Gets a listing stock dependence type by given ID.
      operationId: getRestListingsStockDependenceTypes
      x-api-path-slug: restlistingsstock-dependence-typesid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Stock
      - Dependence
      - Type
  /rest/listings/types:
    get:
      summary: List listing types
      description: Lists all listing types.
      operationId: getRestListingsTypes
      x-api-path-slug: restlistingstypes-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Types
  /rest/listings/types/{id}:
    get:
      summary: Get a listing type
      description: Gets a listing type by given ID.
      operationId: getRestListingsTypes
      x-api-path-slug: restlistingstypesid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Type
  /rest/listings/{id}:
    delete:
      summary: Delete a listing
      description: Deletes a listing by given ID.
      operationId: deleteRestListings
      x-api-path-slug: restlistingsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listing
    get:
      summary: Get a listing
      description: Gets a listing by given ID.
      operationId: getRestListings
      x-api-path-slug: restlistingsid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Listing
    put:
      summary: Update a listing
      description: Updates a listing by given ID.
      operationId: putRestListings
      x-api-path-slug: restlistingsid-put
      parameters:
      - in: body
        name: /rest/listings/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listing
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