---
description: >-
  Once Baxtersweb Maps is installed and configured, you can begin creating
  interactive maps for your website.
---

# Usage

### Creating a Map

Create or edit the post, page or custom post type where you want your map to appear.

Using the Baxtersweb Maps fields, add your route points and points of interest. As you save your content, the map data is stored alongside your post, making it easy to update whenever required.

### Route Points

Route points define the path of your journey.

Add each point in the order it should appear on the map.

If a routing API key is configured, Baxtersweb Maps will calculate the road route between each point. Otherwise, route points are connected using a dashed straight line.

### Points of Interest

Points of interest (POIs) highlight important locations along your route.

Unlike route points, POIs are displayed independently and are not used when calculating the route.

POIs are ideal for highlighting attractions, accommodation, restaurants, landmarks and other useful locations.

### Displaying a Map

Display a map anywhere on your website using the shortcode:

```
[bxtr_map]
```

If you're displaying maps inside a loop or custom template, pass the appropriate post ID to display the correct map.

### Customising Maps

The appearance of your maps can be customised from **Maps → Setup**.

Available options include:

* Route colours
* Marker colours
* Marker labels
* POI marker styles
* Border radius
* Route numbering
* Nearby POI grouping

See the **Setup** guide for a complete explanation of each option.

### Best Practices

For the best results:

* Add route points in travel order.
* Use clear, descriptive labels for points of interest.
* Only include locations that add value to the visitor.
* Keep maps focused on a single journey or area.

### Next Steps

Now that you know how to create maps, you can:

* Configure routing and styling options in [**Setup**](setup.md).
* Explore practical examples in [**Examples**](examples.md).
* Visit [**FAQ**](faq.md) and [**Troubleshooting**](troubleshooting.md) if you need additional help.
