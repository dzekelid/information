---
swagger: "2.0"
x-collection-name: Coord
x-complete: 0
info:
  title: Coord Bike Share API Get information on all bike systems in an area, as a
    GeoJSON FeatureCollection.
  description: |-
    Bike systems are individual bike share systems, often per-region.

    Information about each system is returned as a GeoJSON Feature, within a single GeoJSON
    FeatureCollection.

    See the [/system/{system_id}](#reference/0/get-information-for-a-bike-system) call for more
    details on the individual system Features.

    ### Example

    #### Request:
    `curl -G "https://api.coord.co/v1/bike/system?latitude=40.74286877312112&longitude=-73.98918628692627&radius_km=0.5&access_key="`

    #### Response:
    ```
    {
      "features": [
        {
          "geometry": {
            "coordinates": [
              [
                [
                  [
                    -74.055701,
                    40.707838
                  ],
                  [
                    -74.083639,
                    40.714807
                  ],
                  ...,
                  [
                    -74.055701,
                    40.707838
                  ]
                ]
              ]
            ],
            "type": "MultiPolygon"
          },
          "id": "CitiBike",
          "properties": {
            "is_transactable": true,
            "station_type": "dock"
          },
          "type": "Feature"
        }
      ],
      "type": "FeatureCollection"
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
  /system:
    get:
      summary: Get information on all bike systems in an area, as a GeoJSON FeatureCollection.
      description: |-
        Bike systems are individual bike share systems, often per-region.

        Information about each system is returned as a GeoJSON Feature, within a single GeoJSON
        FeatureCollection.

        See the [/system/{system_id}](#reference/0/get-information-for-a-bike-system) call for more
        details on the individual system Features.

        ### Example

        #### Request:
        `curl -G "https://api.coord.co/v1/bike/system?latitude=40.74286877312112&longitude=-73.98918628692627&radius_km=0.5&access_key="`

        #### Response:
        ```
        {
          "features": [
            {
              "geometry": {
                "coordinates": [
                  [
                    [
                      [
                        -74.055701,
                        40.707838
                      ],
                      [
                        -74.083639,
                        40.714807
                      ],
                      ...,
                      [
                        -74.055701,
                        40.707838
                      ]
                    ]
                  ]
                ],
                "type": "MultiPolygon"
              },
              "id": "CitiBike",
              "properties": {
                "is_transactable": true,
                "station_type": "dock"
              },
              "type": "Feature"
            }
          ],
          "type": "FeatureCollection"
        }
        ```
      operationId: search_bike_systems
      x-api-path-slug: system-get
      parameters:
      - in: query
        name: access_key
        description: The API access key for the request
      - in: query
        name: latitude
        description: Latitude to return results for
      - in: query
        name: longitude
        description: Longitude to return results for
      - in: query
        name: radius_km
        description: Distance, in kilometers, from (latitude, longitude) we will return
          results for
      responses:
        200:
          description: OK
      tags:
      - Information
      - "On"
      - ""
      - Bike
      - Systems
      - In
      - Area
      - ""
      - As
      - GeoJSON
      - FeatureCollection
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