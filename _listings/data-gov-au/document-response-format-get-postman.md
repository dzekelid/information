{
  "info": {
    "name": "Regulations.gov Returns Document information",
    "_postman_id": "234788fd-fbad-4c09-821a-46bfbe816df3",
    "description": "Returns document information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Returns",
      "item": [
        {
          "id": "9bc96254-c3d8-4186-a604-2358b132b5d5",
          "name": "getDocument.ResponseFormat",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.data.gov",
              "path": [
                "regulations",
                "v3",
                "document.:response_format"
              ],
              "query": [
                {
                  "key": "documentId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "federalRegisterNumber",
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
            "description": "Returns document information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6c4bf8c-3099-4b2c-836b-fc71cd8f258a"
            }
          ]
        }
      ]
    }
  ]
}