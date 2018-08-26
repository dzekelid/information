{
  "info": {
    "name": "Bitly Link API Get Info",
    "_postman_id": "e766f2e8-6a6e-43b5-84c0-a0eb5ea03a57",
    "description": "Get info.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Search",
      "item": [
        {
          "id": "e954ada5-2ec7-4444-931e-d799d6642121",
          "name": "getSearch",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/search?cities=%7B%7D&domain=%7B%7D&fields=%7B%7D&full_domain=%7B%7D&lang=%7B%7D&limit=%7B%7D&offset=%7B%7D&query=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get search."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc5bedcb-37f7-4e2c-990d-6ed28ce49519"
            }
          ]
        }
      ]
    },
    {
      "name": "Expand",
      "item": [
        {
          "id": "d371cc30-ac68-446c-8120-ac1c53c9e894",
          "name": "getV3Expand",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/expand?format=%7B%7D&hash=%7B%7D&shortUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get expand."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b8a033c-3904-4da3-8c91-f945a19053f8"
            }
          ]
        }
      ]
    },
    {
      "name": "Info",
      "item": [
        {
          "id": "c9da73b8-104b-4b21-8285-bf8a46d1a790",
          "name": "getV3Info",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/info?expand_user=%7B%7D&hash=%7B%7D&shortUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get info."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb522b6b-851f-4bfd-9a3f-2b88159567ec"
            }
          ]
        }
      ]
    }
  ]
}