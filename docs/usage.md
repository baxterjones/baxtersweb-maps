---
description: >-
  Once Baxtersweb Maps has been installed and configured, you're ready to start
  creating interactive maps.
---

# Usage

This guide explains the basic workflow, from creating a route to displaying it on your website.

### The Workflow

Using Baxtersweb Maps follows four simple steps:

1. Create or edit a post, page or custom post type.
2. Add your route points and points of interest using the Baxtersweb Maps fields.
3. Save or update your content.
4. Display the map using the `[bxtr_map]` shortcode.

### Creating a Map

Open the content where you'd like your map to appear.

You'll find the Baxtersweb Maps field group, where you can add:

* Route points
* Points of interest
* Labels
* Descriptions
* Images

Each route point is displayed in the order it appears, allowing you to create journeys, itineraries and guided routes.

### Displaying a Map

To display the map, simply add the shortcode where you'd like it to appear.

```
[bxtr_map]
```

When used within a single post or page, the shortcode automatically displays the map for the current content.

### Using the Shortcode in Loops

When displaying maps inside archive pages or custom loops, provide the current post ID.

For example:

```
echo do_shortcode( '[bxtr_map id="' . get_the_ID() . '"]' );
```

If you're using Advanced Views or another templating solution, pass the current object ID to the shortcode.

### Route Points

Route points create the line connecting locations.

Each point can include:

* Location
* Title
* Description
* Image

The order of the points determines the route displayed on the map.

### Points of Interest

Points of interest (POIs) highlight important locations without becoming part of the route.

Common uses include:

* Accommodation
* Restaurants
* Attractions
* Parking
* Information centres
* Meeting points

POIs can be displayed alongside a route or independently.

### Customising the Map

Baxtersweb Maps includes several options for customising the appearance of your maps, including:

* Map height
* Route colour
* Marker colour
* Label styles

For a complete explanation of every option, continue to the **Setup** guide.

### Next Steps

Now that you understand the basic workflow, explore the following guides:

* [**Setup**](setup.md) — customise the appearance and behaviour of your maps.
* [**Examples**](examples.md) — discover practical ways to use Baxtersweb Maps.
* [**FAQ**](faq.md) — answers to common questions.
* [**Troubleshooting**](troubleshooting.md) — resolve common issues.
