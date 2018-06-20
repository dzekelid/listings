{
  "info": {
    "name": "Etsy Get Shops Shop Listings Inactive Listing",
    "_postman_id": "4f792916-280c-49c4-a805-f1cc03182e52",
    "description": "Retrieves a Listing associated to a Shop that is inactive",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Home Pages",
      "item": [
        {
          "id": "cab37be1-545b-4393-996a-d849ed025d59",
          "name": "getHomepagesPickersFeaturedListingPickerListingsActive",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "homepages/pickers/:featured_listing_picker_id/listings/active"
              ],
              "variable": [
                {
                  "id": "featured_listing_picker_id",
                  "value": "featured_listing_picker_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of Listing objects associated to a FeaturedListingPicker in scope active."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "804ef472-0f01-4c28-a030-44a262a5b671"
            }
          ]
        },
        {
          "id": "a77bd71c-1991-4c96-b94b-1f3364d183b2",
          "name": "getHomepagesListingsActive",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/homepages/listings/active",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all FeaturedListings that point to active Listings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2a5f6d2-2ee3-4330-865c-640c81c69bea"
            }
          ]
        }
      ]
    },
    {
      "name": "Listings",
      "item": [
        {
          "id": "007aea5a-0ab2-47ee-bfe4-7ddde9ca8b7a",
          "name": "getListingsActive",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/listings/active",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all active Listing"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8791afd1-df4a-4a09-9a0b-37ae5003ff00"
            }
          ]
        }
      ]
    },
    {
      "name": "Shops",
      "item": [
        {
          "id": "da8d59d0-d958-4504-88c5-b4c291f46fbd",
          "name": "getShopsShopListingsActive",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shops/:shop_id/listings/active"
              ],
              "variable": [
                {
                  "id": "shop_id",
                  "value": "shop_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all active Listings associated with a Shop"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85d73bbb-1c0e-48ad-84ef-b0d7743489c3"
            }
          ]
        },
        {
          "id": "0693b2e3-5a6e-4e3a-9f4f-30e7b5097b83",
          "name": "getShopsShopListingsInactive",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shops/:shop_id/listings/inactive"
              ],
              "variable": [
                {
                  "id": "shop_id",
                  "value": "shop_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves Listings associated to a Shop that are inactive"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "079e9f81-5f75-4ad2-b7de-6151d25a6110"
            }
          ]
        },
        {
          "id": "09748d63-d230-4d52-bad4-d8082ad90a39",
          "name": "getShopsShopListingsInactiveListing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "shops/:shop_id/listings/inactive/:listing_id"
              ],
              "variable": [
                {
                  "id": "shop_id",
                  "value": "shop_id",
                  "type": "string"
                },
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a Listing associated to a Shop that is inactive"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24fd7c8b-dd35-4005-b50b-71ee559833cb"
            }
          ]
        }
      ]
    }
  ]
}