{
  "info": {
    "name": "reverb Get Listings",
    "_postman_id": "0e47e8ca-2c9e-475d-8afb-8c477a98c0a3",
    "description": "Default search of listings includes only used & handmade. Add a filter to view all listings or use the /listings/all endpoint.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Comparison",
      "item": [
        {
          "id": "477fc53c-e46b-4852-ae82-05d60580d47a",
          "name": "getComparisonShoppingPagesListings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reverb.com",
              "path": [
                "api",
                "comparison_shopping_pages/:id/listings"
              ],
              "query": [
                {
                  "key": "condition",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "per_page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return new or used listings for a comparison shopping page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86fad876-830e-4655-9545-8c0d0c769b7b"
            }
          ]
        }
      ]
    },
    {
      "name": "Listings",
      "item": [
        {
          "id": "35830736-0ef9-4981-a30b-d46f518560df",
          "name": "getListings",
          "request": {
            "url": "http://api.reverb.com/api/listings?accepts_gift_cards=%7B%7D&accepts_payment_plans=%7B%7D&auction_price_max=%7B%7D&category=%7B%7D&conditions=%7B%7D&currency=%7B%7D&decade=%7B%7D&exclude_auctions=%7B%7D&finish=%7B%7D&handmade=%7B%7D&item_city=%7B%7D&item_country=%7B%7D&item_region=%7B%7D&item_state=%7B%7D&listing_type=%7B%7D&make=%7B%7D&model=%7B%7D&must_not=%7B%7D&not_ids=%7B%7D&offset=%7B%7D&page=%7B%7D&per_page=%7B%7D&preferred_seller=%7B%7D&price_max=%7B%7D&price_min=%7B%7D&product_type=%7B%7D&query=%7B%7D&ships_to=%7B%7D&shop=%7B%7D&shop_id=%7B%7D&watchers_count_min=%7B%7D&year_max=%7B%7D&year_min=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Default search of listings includes only used & handmade. Add a filter to view all listings or use the /listings/all endpoint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "546ee2bc-3713-4afb-b614-5bb04692dc78"
            }
          ]
        }
      ]
    }
  ]
}