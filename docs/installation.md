---
description: This guide explains how to install Baxtersweb Maps and prepare it for use.
---

# Installation

Before continuing, ensure your website meets the requirements listed in the [**Requirements**](requirements.md) guide.

### Install the Plugin

1. Download the latest version of Baxtersweb Maps.
2. Log in to your WordPress admin area.
3. Navigate to **Plugins → Add New Plugin**.
4. Click **Upload Plugin**.
5. Select the Baxtersweb Maps ZIP file.
6. Click **Install Now**.
7. Activate the plugin.

Once activated, you'll find **Maps** in the WordPress admin menu.

### Install the Required Plugins

Baxtersweb Maps requires the following plugins:

* Advanced Custom Fields Pro (ACF Pro)
* ACF OpenStreetMap Field

If either plugin is inactive, Baxtersweb Maps cannot create or display maps correctly.

### Create the Required ACF Fields

After activating the plugin, navigate to:

**Maps → Setup**

Before creating the required fields, decide where they should be stored.

You can either:

* Create a new ACF Field Group specifically for Baxtersweb Maps.
* Add the required fields to one of your existing ACF Field Groups.

#### Create a New Field Group

This option is recommended for new installations.

Enter a name for the field group and click **Create ACF Fields**.

The plugin will automatically create all required fields.

#### Use an Existing Field Group

If you already have an ACF Field Group assigned to your content, you can add the Baxtersweb Maps fields to that group instead.

Select the field group from the list and click **Create ACF Fields**.

This allows your existing custom fields and map fields to be managed together.

### Configure Your Field Group

If you created a new field group, or selected an existing one, make sure its **Location Rules** are configured correctly within ACF.

The field group should be assigned to the post types where you intend to create maps, such as:

* Posts
* Pages
* Custom Post Types
* Tours
* Destinations
* Events

Without the correct location rules, the map fields won't appear when editing your content.

### Verify the Installation

Your installation is complete when:

* Baxtersweb Maps appears in the WordPress admin menu.
* The required ACF fields have been created.
* Your selected field group is assigned to the appropriate content types.
* The map fields are visible when editing your content.

### Next Steps

With the plugin successfully installed, continue to the **Usage** guide to create and display your first interactive map.
