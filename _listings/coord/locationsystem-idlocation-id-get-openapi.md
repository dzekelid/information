---
swagger: "2.0"
x-collection-name: Coord
x-complete: 0
info:
  title: Coord Bike Share API Get detailed information on a bike location, as a GeoJSON
    Feature.
  description: |-
    A bike location may be a single bike station (which can have multiple docked bikes) or a
    single dockless bike itself. All working docks are returned, but only free and rentable
    dockless bikes are returned.

    ### Example

    #### Request:
    `curl -G "https://api.coord.co/v1/bike/location/CitiBike/482?access_key="`

    #### Response:
    ```
    {
      "geometry": {
        "coordinates": [
          -73.99931783,
          40.73935542
        ],
        "type": "Point"
      },
      "id": "CitiBike-482",
      "properties": {
        "is_renting": true,
        "is_returning": true,
        "last_reported": "2018-05-17T15:41:06.000Z",
        "lat": 40.73935542,
        "location_id": "482",
        "location_type": "bike_station_dock",
        "lon": -73.99931783,
        "name": "W 15 St & 7 Ave",
        "num_bikes_available": 19,
        "num_docks_available": 19,
        "region_id": "71",
        "system_id": "CitiBike"
      },
      "type": "Feature"
    }
    ```
  version: 1.0.0
host: api.coord.co
basePath: /v1/bike
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /location/{system_id}/{location_id}:
    get:
      summary: Get detailed information on a bike location, as a GeoJSON Feature.
      description: |-
        A bike location may be a single bike station (which can have multiple docked bikes) or a
        single dockless bike itself. All working docks are returned, but only free and rentable
        dockless bikes are returned.

        ### Example

        #### Request:
        `curl -G "https://api.coord.co/v1/bike/location/CitiBike/482?access_key="`

        #### Response:
        ```
        {
          "geometry": {
            "coordinates": [
              -73.99931783,
              40.73935542
            ],
            "type": "Point"
          },
          "id": "CitiBike-482",
          "properties": {
            "is_renting": true,
            "is_returning": true,
            "last_reported": "2018-05-17T15:41:06.000Z",
            "lat": 40.73935542,
            "location_id": "482",
            "location_type": "bike_station_dock",
            "lon": -73.99931783,
            "name": "W 15 St & 7 Ave",
            "num_bikes_available": 19,
            "num_docks_available": 19,
            "region_id": "71",
            "system_id": "CitiBike"
          },
          "type": "Feature"
        }
        ```
      operationId: get_bike_location
      x-api-path-slug: locationsystem-idlocation-id-get
      parameters:
      - in: query
        name: access_key
        description: The API access key for the request
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Detailed
      - Information
      - "On"
      - Bike
      - Location
      - ""
      - As
      - GeoJSON
      - Feature
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---