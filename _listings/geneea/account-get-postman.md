{
  "info": {
    "name": "Geneea Natural Language Processing Get Account",
    "_postman_id": "77f23d7e-9bb1-40f3-b35b-bbedee9bf7f6",
    "description": "Information about current user account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "b27510b1-6e90-4af1-bcde-fd5cb8e3cb4b",
          "name": "getAccount",
          "request": {
            "url": "http://api.geneea.com/account",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Information about current user account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4213934-7238-4c64-819e-f339e512307e"
            }
          ]
        }
      ]
    }
  ]
}