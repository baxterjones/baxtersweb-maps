---
description: Diagnose missing fields, empty maps, routing failures and display problems.
icon: lightbulb-exclamation-on
---

# Troubleshooting

## The Baxtersweb Maps fields do not appear

1. Confirm ACF Pro and ACF OpenStreetMap Field are active.
2. Open **Tools → Baxtersweb Maps → Overview** and check the map field status.
3. If using the generated group, confirm the required post type was selected during setup.
4. If using an existing group, review that group's ACF location rules.
5. Click **Add or update missing fields** if the setup is incomplete.

## The map does not appear

A map needs at least one valid route marker or POI after visibility settings are applied.

Check that:

* The shortcode is on a page where the intended post can be detected, or includes the correct `id`.
* At least one location field contains valid raw coordinate data.
* POIs have not been disabled when the map contains only POIs.
* The route has not been disabled when the map contains only route markers.

## The wrong map appears in a loop

Pass the current item's ID explicitly:

```php
echo do_shortcode('[bxtr_map id="' . get_the_ID() . '"]');
```

For Advanced Views:

```text
[bxtr_map id="{{ _layout.object_id }}"]
```

## A route line does not appear

A route requires at least two unique, valid route marker locations and route visibility must be enabled.

With no API key, the expected result is a dashed straight line. With a connected key, the plugin uses saved road geometry when available.

## Road routing fails

Open **Tools → Baxtersweb Maps → Routing** and review the saved connection status.

Common causes include:

* An invalid or inactive openrouteservice API key.
* API usage limits.
* The server blocking outgoing HTTPS requests.
* A marker too far from a mapped drivable road.
* A route that the service cannot calculate.

The plugin retries the specific road-snapping failure with a 2 km limit and can split longer multi-stop requests into legs, but some coordinates still cannot produce a road route.

Editors who can edit the affected post may see the saved routing error above the map. Visitors receive the normal fallback behaviour rather than that diagnostic.

## A changed route still shows old geometry

Save or update the post after changing marker coordinates. The plugin compares a coordinate hash and requests new geometry when the ordered unique coordinates change.

If necessary, reconnect a valid API key to refresh maps that have no saved geometry.

## POIs are missing

Check that:

* POI fields were included during field setup.
* POI visibility is enabled globally or with `poi="yes"`.
* Each POI contains one valid location.
* The shortcode has not set `poi="no"`.

## Nearby POIs appear as one marker

This is POI grouping. Click the grouped marker to spread the locations, or disable **Group nearby POIs** under **Styles**.

## Colours or dimensions revert to defaults

Colour values must be valid hex colours. Map height accepts `px`, `vh`, `vw`, `rem` or `em`; border radius also accepts `%`. Invalid values are replaced with plugin defaults when saved.

Clear page and browser caches after saving style changes.

## JavaScript or layout conflicts

Test with caching and optimisation disabled, then check the browser console. If the issue remains, temporarily test with a default theme and only the required plugins active.

When requesting support, provide the page URL, plugin version, WordPress and PHP versions, browser console errors, and exact reproduction steps.
