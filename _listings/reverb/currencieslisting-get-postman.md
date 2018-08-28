{
  "info": {
    "name": "reverb Get Currencies Listing",
    "_postman_id": "57af807a-d8aa-419c-b387-eebd882f1ca7",
    "description": "List of supported listing currencies for shops",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Currencies",
      "item": [
        {
          "id": "9ed1ddcc-24ca-48e0-82a3-a19b384c5bcb",
          "name": "getCurrenciesDisplay",
          "request": {
            "url": "http://api.reverb.com/api/currencies/display",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of supported display currencies for browsing listings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08560930-150a-490c-b1ef-ba3d426bbbbc"
            }
          ]
        },
        {
          "id": "31668fbe-570d-4a2d-92c2-5539c2c053db",
          "name": "getCurrenciesListing",
          "request": {
            "url": "http://api.reverb.com/api/currencies/listing",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of supported listing currencies for shops"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fabc70b3-8637-484f-a81c-91c03366efbd"
            }
          ]
        }
      ]
    }
  ]
}