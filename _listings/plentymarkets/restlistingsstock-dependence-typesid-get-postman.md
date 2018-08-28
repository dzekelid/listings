{
  "info": {
    "name": "Plentymarkets Get a listing stock dependence type",
    "_postman_id": "abc96dff-1852-4b44-b0a6-16841f83072d",
    "description": "Gets a listing stock dependence type by given ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "f3ec960a-f5c3-4376-a3c8-9f7a6162270e",
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
              "id": "5d00add0-f329-4a12-b5c4-5a09d6d3c7ea"
            }
          ]
        }
      ]
    },
    {
      "name": "Listing",
      "item": [
        {
          "id": "bf241388-a271-44f7-b4c1-63bedf4ac88b",
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
              "id": "4354a15d-7a83-4903-b2b8-8f05e25ea121"
            }
          ]
        }
      ]
    }
  ]
}