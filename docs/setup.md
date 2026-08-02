---
description: Configure fields, routing, map styles and uninstall behaviour.
icon: gear
---

# Setup

Baxtersweb Maps is managed from **Tools → Baxtersweb Maps**. Its four tabs separate field setup, routing, appearance and data preferences.

## Overview

### Setup status

The status table checks:

* ACF Pro.
* ACF OpenStreetMap Field.
* Whether the Baxtersweb Maps route fields exist.
* Whether optional road routing is connected.

### Add map fields

Choose one field group mode:

**Create a new field group**

The plugin creates or updates **Baxtersweb Maps Fields** and assigns it to the selected public post types. Posts and pages are selected by default when available.

**Add fields to an existing group**

Choose an existing ACF field group. The plugin adds or updates only its own stable fields and does not rename, map or remove your other fields.

Route marker fields are always created. POI fields are optional. Re-running the setup updates missing Baxtersweb Maps fields rather than duplicating them.

### Display reference

The Overview tab also shows the standard shortcode and examples for specific content IDs, PHP templates and Advanced Views.

## Routing

Baxtersweb Maps uses **openrouteservice** for optional road-following geometry.

1. Create an openrouteservice API key.
2. Paste it into the Routing tab.
3. Click **Save & Test API**.

When the key is verified, the plugin attempts to calculate routes for existing maps that do not yet have saved road geometry. New or changed routes are calculated when their content is saved.

Calculated geometry is stored in post meta and reused. Removing the API key keeps existing saved road routes, but new or changed routes use the straight-line fallback until another valid key is connected.

For rural markers that cannot be matched within the service's normal range, the plugin retries with a bounded 2 km road-snapping radius. Longer multi-stop routes may be requested one leg at a time and merged.

## Styles

Styles are global defaults for all maps.

### Route and map

* **Show route line** — enable or disable the line between route markers.
* **Route colour** — colour of the road route or fallback line.
* **Route marker colour** — marker background.
* **Route marker text colour** — letter or number colour.
* **Marker sequence** — alphabetical or numeric.
* **Map height** — accepts `px`, `vh`, `vw`, `rem` or `em`, for example `500px` or `70vh`.
* **Border radius** — accepts the same units plus `%`.

### Points of interest

* **Show points of interest** — global POI visibility.
* **POI marker colour** — default background colour.
* **POI icon mode** — built-in Dashicon, theme icon class or plain marker.
* **Default icon** — used when built-in icons are selected.
* **Theme icon class** — default CSS class when theme icons are selected.
* **Group nearby POIs** — combines close locations and spreads them when clicked.

Individual POI rows can override the global icon or background colour when the corresponding generated fields are present.

The live preview reflects the saved style settings.

## Help & Data

This tab contains documentation and demo links, the field-name reference, shortcode examples and the uninstall preference.

### Data on uninstall

Choose whether deleting the plugin should:

* Keep plugin settings and generated fields; or
* Remove plugin settings and the dedicated generated **Baxtersweb Maps Fields** group.

Fields added to another ACF field group are not removed with that group. Existing post content is not described as being deleted by this setting.
