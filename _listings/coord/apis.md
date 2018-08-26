---
name: Coord
x-slug: coord
description: Coord is a mobility company that creates seamless mobility and self-driving
  experiences today through deep integrations. The company offers bike-share API,
  Curbs API, Tolls API, Routing API and etc.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
x-kinRank: "7"
x-alexaRank: "1035226"
tags: Information
created: "2018-08-25"
modified: "2018-08-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/information/master/_listings/coord/apis.md
specificationVersion: "0.14"
apis:
- name: Bike Share API - Get detailed information on a bike location, as a GeoJSON
    Feature.
  x-api-slug: locationsystem-idlocation-id-get
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/bike
  tags: Parking, Tolls, Bikes, Routes, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/information/master/_listings/coord/locationsystem-idlocation-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/information/master/_listings/coord/locationsystem-idlocation-id-get-openapi.md
- name: Bike Share API - Get information on all bike systems in an area, as a GeoJSON
    FeatureCollection.
  x-api-slug: system-get
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/bike
  tags: Parking, Tolls, Bikes, Routes, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/information/master/_listings/coord/system-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/information/master/_listings/coord/system-get-openapi.md
- name: Bike Share API - Get detailed information on a bike system, as a GeoJSON feature.
  x-api-slug: systemsystem-id-get
  description: |-
    Bike systems are individual bike share systems, often per-region.

    Information is returned as a GeoJSON Feature. The geometry of the GeoJSON Feature is
    a MultiPolygon that defines the system's operational area. All bike systems have an
    operational area, in which bikes may be found and parked.
    For systems that require bikes be docked, this area is somewhat arbitrary, as bikes are
    only found at stations. In this case, the operational area is roughly the city or
    jurisdiction that the system covers.
    For semi-dockless and dockless systems that allow bikes to be parked anywhere, the
    operational area is very important and strictly defined. Often there are extra fees for
    parking outside of the operational area (also known as a "catchment area"), and almost all
    bikes should be within the area.

    These bike system types are reflected in the `station_type` property.
    * `dock` - All bikes must be taken from and returned to a dock.
    * `dockless` - All bikes are only dockless.
    * `dockless_with_hub` - Bikes may be dockless, or taken from or returned to a hub.
    A hub can be an area rather than a discrete station, where a bike can be returned and
    locked but not explicitly docked. The total price of a rental may change based on whether
    a bike is returned to a hub or not.

    Areas are returned as a GeoJSON MultiPolygon since areas may be discontiguous or have
    holes.

    ### Example

    #### Request:
    `curl -G "https://api.coord.co/v1/bike/system/CitiBike?access_key="`

    #### Response:
    ```
    {
      "type": "Feature",
      "geometry": {
          "type": "MultiPolygon",
          "coordinates": [
            [
              [ [-74.00, 40.70], [-74.00, 40.80], [-73.90, 40.80], ..., [-74.00, 40.70] ]
            ],
            ...,
            [
              [ [-73.00, 41.70], [-73.00, 41.80], [-72.90, 41.80], ..., [-73.00, 41.70] ],
              [ [-72.98, 41.75], [-72.98, 41.78], [-72.95, 41.78], ..., [-72.98, 41.75] ]
            ]
          ]
        },
      "id": "CitiBike",
      "properties": {
        "email": "support@coord.co",
        "phone_number": "+6789998212",
        "station_type": "dock",
        "is_transactable": "false"
      }
    }
    ```
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/coord-logo.png
  humanURL: https://coord.co
  baseURL: https://api.coord.co//v1/bike
  tags: Parking, Tolls, Bikes, Routes, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/information/master/_listings/coord/systemsystem-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/information/master/_listings/coord/systemsystem-id-get-openapi.md
x-common:
- type: x-blog
  url: https://medium.com/coord
- type: x-blog-rss
  url: https://medium.com/feed/coord
- type: x-openapi
  url: https://jsapi.apiary.io/apis/coordprodsearchtolls.source
- type: x-api-gallery
  url: http://convertapi.api.gallery.streamdata.io
- type: x-api-stack
  url: http://coord.stack.network
- type: x-developer
  url: https://coord.co/docs/
- type: x-pricing
  url: https://coord.co/#pricing
- type: x-twitter
  url: https://twitter.com/coordcity
- type: x-website
  url: https://coord.co
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---