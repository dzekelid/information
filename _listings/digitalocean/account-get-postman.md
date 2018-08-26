{
  "info": {
    "name": "Digital Ocean Get User Information",
    "_postman_id": "aa0eb85e-2f5a-4d85-9c6f-fd62adab2dea",
    "description": "Get [DigitalOcean](https://www.digitalocean.com/) account",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "17b8ec82-0f25-441a-9056-278f1e139334",
          "name": "AccountGet",
          "request": {
            "url": "http://example.com/account",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get [DigitalOcean](https://www.digitalocean.com/) account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d95e00e4-03bb-4cfb-a0dd-46d567abc8e9"
            }
          ]
        }
      ]
    }
  ]
}