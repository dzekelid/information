{
  "info": {
    "name": "Vinli Get Info about a DTC",
    "_postman_id": "cbf687c5-d55e-49c0-9eca-3eed9619f2f3",
    "description": "Get info about a dtc.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Info",
      "item": [
        {
          "id": "d3a63abb-a064-46d0-b505-ac4aeec0f105",
          "name": "CodesGet",
          "request": {
            "url": "http://events.vin.li/api/v1/codes?number=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get info about a dtc."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75003b4c-eefb-408a-afa4-0143ad5b53ac"
            }
          ]
        }
      ]
    }
  ]
}