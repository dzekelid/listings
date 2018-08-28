{
  "info": {
    "name": "Plentymarkets List listing stock dependence types",
    "_postman_id": "adfc66d5-61dc-4c63-acc3-6792cac0b86e",
    "description": "Lists listing stock dependence types.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "abaf4408-d914-40eb-aa2e-8f20702894c1",
          "name": "getRestListingsStockDependenceTypes",
          "request": {
            "url": "http://example.com/rest/listings/stock_dependence_types?itemsPerPage=%7B%7D&page=%7B%7D&with=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists listing stock dependence types."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f399c05-fcda-4a86-8a74-3ea8f0a257cc"
            }
          ]
        }
      ]
    },
    {
      "name": "Listing",
      "item": [
        {
          "id": "92c9e181-20c2-49a2-bc04-fa5ae838d277",
          "name": "getRestListingsStockDependenceTypes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/listings/stock_dependence_types/:id"
              ],
              "query": [
                {
                  "key": "with",
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
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets a listing stock dependence type by given ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4a3d079-d8b1-4490-af22-b383ebc1ac63"
            }
          ]
        }
      ]
    }
  ]
}