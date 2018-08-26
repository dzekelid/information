{
  "info": {
    "name": "Regulations.gov Returns Docket information",
    "_postman_id": "c13582fc-4d31-40b3-968f-bc8f717b5ed4",
    "description": "Returns docket information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Returns",
      "item": [
        {
          "id": "c72625bc-05c5-423e-a0b4-9dd8f4b50c72",
          "name": "getDocket.ResponseFormat",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.data.gov",
              "path": [
                "regulations",
                "v3",
                "docket.:response_format"
              ],
              "query": [
                {
                  "key": "docketId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "response_format",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns docket information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ccf0e94-d9a0-4e4f-9b0e-1dbbdc5b7b9c"
            }
          ]
        }
      ]
    }
  ]
}