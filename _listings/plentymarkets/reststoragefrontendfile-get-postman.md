{
  "info": {
    "name": "Plentymarkets Get file information for a single object in frontend storage. Append public cloudfront url to retrieved object.",
    "_postman_id": "f14e52c9-9c0b-4b6e-ac1e-52b82b4a4cf8",
    "description": "Get file information for a single object in frontend storage. append public cloudfront url to retrieved object..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "File",
      "item": [
        {
          "id": "afddec1a-aa99-4940-8494-c72d5efa81ce",
          "name": "getRestStorageFrontendFile",
          "request": {
            "url": "http://example.com/rest/storage/frontend/file?key=%7B%7D",
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
            "description": "Get file information for a single object in frontend storage. append public cloudfront url to retrieved object.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55571498-ad10-4e65-a4d0-2109cd480ee0"
            }
          ]
        }
      ]
    }
  ]
}