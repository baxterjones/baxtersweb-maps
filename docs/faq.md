---
description: Answers to common questions about Baxtersweb Maps.
icon: messages-question
---

# FAQ

<details>
<summary>Does Baxtersweb Maps require ACF Pro?</summary>

Yes. The plugin uses ACF Pro repeater fields for route markers and optional points of interest.
</details>

<details>
<summary>Is ACF OpenStreetMap Field required?</summary>

Yes. It provides the location picker used in each map row.
</details>

<details>
<summary>Do I need a Google Maps API key?</summary>

No. Maps use OpenStreetMap tiles and Leaflet.
</details>

<details>
<summary>Do I need a routing API key?</summary>

Not for normal maps. Without a key, route markers are joined by a dashed straight line. A valid openrouteservice key is only needed for road-following geometry.
</details>

<details>
<summary>What happens if I remove the routing API key?</summary>

Previously saved road routes remain available. New or changed routes use the straight-line fallback until another valid key is connected.
</details>

<details>
<summary>Can I use custom post types?</summary>

Yes. When creating a new field group, select any available public post types. You can also add the fields to an existing ACF group with its own location rules.
</details>

<details>
<summary>Can I display only points of interest?</summary>

Yes:

```text
[bxtr_map route="no" poi="yes"]
```
</details>

<details>
<summary>Can I display only route markers?</summary>

Yes:

```text
[bxtr_map route="yes" poi="no"]
```
</details>

<details>
<summary>Can I place multiple maps on one page?</summary>

Yes. Each rendered map receives a unique ID. Pass the correct post ID to each shortcode when the maps use different content.
</details>

<details>
<summary>Can I use the shortcode in a page builder or loop?</summary>

Yes. Use `[bxtr_map]` when the current post is unambiguous, or `[bxtr_map id="123"]` when rendering a specific content item.
</details>

<details>
<summary>Does the plugin provide turn-by-turn navigation?</summary>

No. It displays an interactive route overview and location popups. It is not a live navigation system.
</details>

<details>
<summary>Are routes recalculated on every page view?</summary>

No. Road geometry is saved in WordPress and reused. It is recalculated when route coordinates change, when missing routes are refreshed after connecting a valid key, or when an unrouted map first needs geometry.
</details>

<details>
<summary>Can I change one map without changing all maps?</summary>

The `route` and `poi` shortcode attributes provide per-map visibility overrides. Other appearance options are global unless a developer supplies a named configuration through the `bxtr_template_config` filter.
</details>

<details>
<summary>Where can I get support?</summary>

Use the [WordPress.org support forum](https://wordpress.org/support/plugin/baxtersweb-maps/) and include the plugin version, WordPress version, relevant error message and steps to reproduce the issue.
</details>
