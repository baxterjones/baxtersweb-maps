---
icon: stars
---

# Getting Started

This guide will walk you through the essential steps to create and display your first interactive map.

By the end of this guide, you'll have a working map with route points or points of interest displayed on your website.

### Before You Begin

Before continuing, make sure you have:

* WordPress installed.
* ACF Pro installed and activated.
* ACF OpenStreetMap Field installed and activated.
* Baxtersweb Maps installed and activated.

If you haven't installed the plugin yet, follow the [**Installation**](installation.md) guide first.

### Step 1: Create the Map Fields

Go to **Tools → Baxtersweb Maps → Overview**.

Choose one of the following options under Add map fields:

* **Create new field group** to generate a dedicated Baxtersweb Maps Field Group.
* **Add fields to an existing group** to add the Baxtersweb Maps fields to one of your existing ACF Field Groups.

If you're creating a new Field Group, remember to configure the ACF **Location Rules** so the fields appear on the content you want to map.

### Step 2: Create Your Content

Create or edit the post, page or custom post type where you want to display your map.

Complete the Baxtersweb Maps fields by adding:

* Route points
* Points of interest
* Any optional map settings

Publish or update your content when you're finished.

### Step 3: Display the Map

Add the map shortcode where you'd like the map to appear.

```
[bxtr_map]
```

If you're displaying maps inside a loop or template, pass the appropriate post ID. See [**Usage**](usage.md#displaying-a-map).

### Step 4: Improve Your Map

Once your first map is working, you can customise it by:

* Changing colours and marker styles.
* Choosing letters or numbers for route markers.
* Enabling automatic road routing with a free routing API key.
* Adjusting the map appearance to match your website.

> **Note:** If you don't configure a routing API key, Baxtersweb Maps will still connect your route points using a dashed straight line.

### Next Steps

Now that your first map is working, you can explore the rest of the documentation:

* [**Usage**](usage.md) explains how to build maps effectively.
* [**Setup**](setup.md) covers all available configuration options.
* [**Examples**](examples.md) demonstrates common use cases.
* [**Troubleshooting**](troubleshooting.md) helps resolve common issues.
