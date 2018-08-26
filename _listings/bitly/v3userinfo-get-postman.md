{
  "info": {
    "name": "Bitly User API User Info",
    "_postman_id": "4a0d14d2-e9d0-499c-a594-eeffa611a322",
    "description": "Return or update information about a user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "OAuth",
      "item": [
        {
          "id": "3953dcdf-0968-4fb2-88d7-4ad7d11d3258",
          "name": "oauthApp",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/oauth/app?client_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return information about an OAuth app."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b333dd83-7d24-40e8-b4ae-c86749d7b25c"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "9b97182d-9af6-4eab-bac1-91887a5bbcb2",
          "name": "userInfo",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/info?full_name=%7B%7D&login=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return or update information about a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0159a3a4-d26d-423d-b53f-4c7386301c3a"
            }
          ]
        }
      ]
    }
  ]
}