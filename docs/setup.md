---
description: >-
  Baxtersweb Maps is managed from Tools → Baxtersweb Maps in the WordPress
  admin. The plugin includes four tabs that guide you through configuring your
  maps, routing and display settings.
icon: gear
---

# Setup

### Overview

The **Overview** tab helps you prepare your website for creating maps.

From here you can:

* Check that **ACF Pro** is installed and active.
* Check that **ACF OpenStreetMap Field** is installed and active.
* Select or create the ACF field group used for your maps.
* Create the required map fields automatically.
* View the current setup status.

Once your field group has been prepared, you can begin adding maps to your content.

### Routing

The **Routing** tab controls how routes are generated.

By default, Baxtersweb Maps connects markers using straight lines.

If you want roads to be followed automatically, you can connect an OpenRouteService API key.

From this page you can:

* Add or update your API key.
* Test the connection.
* Refresh existing saved routes.
* View the current routing status.

Road-following routing is optional. Without an API key, maps continue to work using straight-line routes.

### Styles

The **Styles** tab controls the default appearance of your maps.

Available options include:

* Route colour.
* Route marker colour.
* Route marker text colour.
* Point of Interest marker colour.
* Default Point of Interest icon.
* Map height.
* Border radius.
* Marker sequence.
* Route visibility.
* Point of Interest visibility.
* Point of Interest clustering.

These defaults are applied to every map unless overridden by shortcode options.

### Help & Data

The **Help & Data** tab provides additional resources and maintenance options.

Here you can:

* View links to the documentation.
* Open the live demo.
* Review the required data structure.
* Configure uninstall behaviour.

This tab is also useful when setting up the plugin on a new website or preparing it for handover.

### Creating the Map Fields

Before creating your first map, you'll need to create the required ACF fields.

From the **Overview** tab:

1. Select an existing ACF Field Group, or create a new one.
2. Click **Create ACF Fields**.
3. The required Route and Point of Interest fields will be added automatically.

You can add these fields to existing content types or use them in a dedicated field group.

### Recommended Workflow

For the best experience:

1. Install the required plugins.
2. Open **Tools → Baxtersweb Maps**.
3. Create the required ACF fields.
4. Configure your preferred map styles.
5. (Optional) Connect OpenRouteService for road-following routes.
6. Add map data to your content.
7. Display the map using the provided shortcode.

Following this workflow ensures your maps are ready to use with minimal configuration.

**Next:** [Examples](examples.md)
