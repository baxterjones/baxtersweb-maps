---
description: Review the required and optional components before installing Baxtersweb Maps.
icon: box-open-full
---

# Requirements

## Required

### WordPress

The plugin readme declares WordPress **6.5 or later**.

### ACF Pro

Baxtersweb Maps requires **Advanced Custom Fields Pro** because route markers and points of interest are stored in repeater fields.

### ACF OpenStreetMap Field

The free **ACF OpenStreetMap Field** plugin provides the location picker used inside each repeater row.

Locations must return **Raw data** and each row should contain one selected marker. Fields created by Baxtersweb Maps use this configuration automatically.

## Optional

### openrouteservice API key

An API key is only needed for road-following routes. Without one, the map still works and uses a dashed straight line between ordered route markers.

### Advanced Views

Advanced Views is not required. The Baxtersweb Maps admin includes an optional integration reference for users who display maps in Advanced Views layouts.

## External connections

When a map is viewed, map tiles are requested from the OpenStreetMap tile service in the visitor's browser. Standard request information, including the visitor's IP address and requested tile coordinates, may be sent to that service.

When road routing is enabled, route coordinates are sent from the WordPress server to openrouteservice when geometry needs to be calculated. The returned route is saved in WordPress and reused on normal page views.

Leaflet, Dashicons and the plugin's own files are loaded locally.
