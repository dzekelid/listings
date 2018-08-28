{
  "info": {
    "name": "reverb Get Comparison Shopping Pages Listings",
    "_postman_id": "e0e65576-aa10-4b8b-8120-f3731476c47d",
    "description": "Return new or used listings for a comparison shopping page",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Comparison",
      "item": [
        {
          "id": "86aa636a-4f5d-4f7f-bebd-49d646baab43",
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
              "id": "967c1031-8648-4d36-8351-637f7a7fb6aa"
            }
          ]
        }
      ]
    }
  ]
}