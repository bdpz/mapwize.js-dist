# CHANGELOG

## Version 2.1

- Migrating to Leaflet 1.0.3 from 0.7. This can bring breaking changes if you are using Leaflet features directly. Please refer to the [Leaflet documentation](http://leafletjs.com/reference-1.0.3.html). 
- Adding multi-point directions. It is now possible to optimize a path with multiple waypoints.
- Adding minZoom param on fitBounds
- Fix bad center on venue zoom on large venues
- Mapwize images (like qrCode and user position button) are now embedded in css
- New direction path style
- [Breaking change] Api.getDirections is now taking an array of waypoints (from, to, waypoints, directionOptions, cb). Backward compatibility has been kept on the map.showDirections function.
- General improvements and bugs fixes

## Version 2.0.2

- Optimized performances deep inside
- Added advanced parser for Mapwize URL
- Added configuration for outdoorMapProvider

## Version 1.7.1

- Renamed Mapwize.api to Mapwize.Api
- Introducing Mapwize.Location service
- Added support for isVisible and isClickable places
- Added support for custom connector icons
- Added callbacks in asynchronous methods

## Version 1.6.1

- Improvements to the initialization sequence
- Demo building now requires an accessKey

## Version 1.6

- Support for multilingual venues
- Support for storing custom "data" on venues, places, placeLists and beacons
- Added callback on Mapwize.map
- Introducing venueEnter and venueExit events

## Version 1.5

- Possibility to request shortest path to list of places (closest place of list is automatically selected)
- Places and layers are displayed at zoom 16 instead of 18
- Improved display of the outdoor places and directions
- Added Mapwize.api methods
- General improvements

## Version 1.4.4

- Bug fix getLayers
- Bug fix setStyle
- Bug fix scroll floor control

## Version 1.4.3

- Bug fix
- Improved caching
- Setting the right user position while loading direction URLs

## Version 1.4.2

- Places are displayed in the order defined on the server.

## Version 1.4.1

- Added possibility to display user heading
- Added a cache system to reduce the network traffic. Use map.refresh to force the refresh of the cache.
- Margins can be set to free the top and bottom of the map.
- Place style can be modifyed in real-time