---
description: Add map content and display it with the Baxtersweb Maps shortcode.
icon: drum
---

# Usage

## Add route markers

Edit a post, page or custom post type containing the Baxtersweb Maps fields.

Under **Map Markers**, add one row per stop. Drag rows into the required route order.

Each row includes:

* **Marker Title** — optional popup heading.
* **Marker Description** — optional popup content.
* **Marker Coordinates** — one location selected in the OpenStreetMap field.

One valid marker displays without a route line. Two or more unique markers can be connected by a saved road route or the dashed straight-line fallback.

Markers at identical coordinates are offset slightly so they remain selectable. Repeated coordinates are ignored when road geometry is requested.

## Add points of interest

POIs are optional and independent from the ordered route. Use them for accommodation, attractions, facilities, landmarks or other supporting places.

Depending on the POI icon mode selected when the fields were generated, a row can include:

* Title and type.
* Description.
* Built-in icon or theme icon override.
* Background colour override.
* One location.

Nearby POIs can be grouped automatically. Clicking a group spreads its markers around the shared area.

## Display the current map

```text
[bxtr_map]
```

The shortcode detects the current post ID.

## Display map data from another post

```text
[bxtr_map id="123"]
```

Use an explicit ID inside loops, reusable templates or anywhere the current content item may be ambiguous.

## Shortcode attributes

| Attribute | Values | Purpose |
| --- | --- | --- |
| `id` | Post ID | Loads map data from a specific post. |
| `route` | `yes` or `no` | Overrides the global route visibility for this map. |
| `poi` | `yes` or `no` | Overrides the global POI visibility for this map. |
| `template` | A sanitised key | Selects a named developer configuration provided through the `bxtr_template_config` filter. |

Examples:

```text
[bxtr_map route="no" poi="yes"]
```

```text
[bxtr_map id="123" route="yes" poi="no"]
```

## PHP template

```php
echo do_shortcode('[bxtr_map id="' . get_the_ID() . '"]');
```

## Advanced Views layout

```text
[bxtr_map id="{{ _layout.object_id }}"]
```

## Page builders

Place the shortcode in a Shortcode, Text or equivalent element. Use an explicit `id` when the builder is rendering another post inside a loop or listing.

## Developer template configurations

The `template` attribute does not load a separate PHP template file. It passes a named key to the `bxtr_template_config` filter, which developers can use to modify the final map configuration.

```php
add_filter('bxtr_template_config', function ($config, $template) {
    if ('compact' === $template) {
        $config['map_height'] = '360px';
        $config['border_radius'] = '0px';
    }

    return $config;
}, 10, 2);
```
