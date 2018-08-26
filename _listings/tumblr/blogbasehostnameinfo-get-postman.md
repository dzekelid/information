{
  "info": {
    "name": "Tumblr Get Blog Base Hostname Info",
    "_postman_id": "e97c140e-11ee-4f77-8221-3bbd3aefc115",
    "description": "This method returns general information about the blog, such as the title, number of posts, and other high-level data.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blog",
      "item": [
        {
          "id": "ab490880-c4f3-4f74-9c77-a01e9737397a",
          "name": "blog.base_hostname.info.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.tumblr.com",
              "path": [
                "v2",
                "blog/:base-hostname/info"
              ],
              "variable": [
                {
                  "id": "base-hostname",
                  "value": "base-hostname",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This method returns general information about the blog, such as the title, number of posts, and other high-level data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63a63e0f-6bdf-48cb-8f03-4fd0547a99d6"
            }
          ]
        }
      ]
    }
  ]
}