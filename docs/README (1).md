---
icon: stars
---

# Getting Started

This guide takes you from activation to a working map.

## 1. Add the map fields

Go to **Tools → Baxtersweb Maps → Overview**.

Choose where the plugin should add its fields:

* **Create a new field group** creates a dedicated **Baxtersweb Maps Fields** group. Select the posts, pages or public custom post types where it should appear.
* **Add fields to an existing group** adds the maintained Baxtersweb Maps fields to a group you already use. The plugin leaves your other fields unchanged.

Route marker fields are always included. Enable **Points of interest** if the map also needs independent locations such as hotels, attractions or facilities.

Click **Add map fields**. You can use the same button later to add or update missing Baxtersweb Maps fields.

## 2. Add map content

Create or edit content where the selected ACF field group appears.

Under **Map Markers**, add one row for each route stop. Set the rows in travel order because the plugin uses that order for the marker sequence and route line.

Each marker can contain:

* A title.
* A description for the popup.
* One location selected in the OpenStreetMap field.

If POI fields were included, add independent locations under **Points of Interest**. POIs do not change the route.

Publish or update the content.

## 3. Display the map

Add the shortcode to the same post or page:

```text
[bxtr_map]
```

To display map data stored on another post, pass its ID:

```text
[bxtr_map id="123"]
```

The map automatically fits the available markers and POIs.

## 4. Optional: enable road routing

Without an API key, two or more route markers are connected by a dashed straight line.

To follow mapped roads instead, go to **Tools → Baxtersweb Maps → Routing**, add an openrouteservice API key, and click **Save & Test API**. Existing maps without saved road geometry are then refreshed automatically.

## 5. Adjust the defaults

Use **Tools → Baxtersweb Maps → Styles** to change colours, height, border radius, marker sequence, route visibility, POI visibility, icons and POI grouping.

See [Usage](usage.md) for shortcode options and [Setup](setup.md) for every admin setting.
