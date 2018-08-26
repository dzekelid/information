{
  "info": {
    "name": "Buffer Get Info Configuration Mediatypeextension",
    "_postman_id": "efabe921-7da5-490d-9cf7-f494451962f9",
    "description": "Returns an object with the current configuration that Buffer is using, including supported services, their icons and the varying limits of character and schedules.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Info",
      "item": [
        {
          "id": "189c8f8d-317b-48b7-a98f-5e3912a1424b",
          "name": "returns-an-object-with-the-current-configuration-that-buffer-is-using-including-supported-services-t",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bufferapp.com",
              "path": [
                "1",
                "info/configuration:mediaTypeExtension"
              ],
              "variable": [
                {
                  "id": "mediaTypeExtension",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an object with the current configuration that Buffer is using, including supported services, their icons and the varying limits of character and schedules."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e731959f-b39f-487c-a761-f23a1a013bc8"
            }
          ]
        }
      ]
    }
  ]
}