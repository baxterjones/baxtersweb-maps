---
description: >-
  If you experience any issues while using Baxtersweb Maps, the following
  solutions may help.
---

# Troubleshooting

### The map doesn't appear

Check the following:

* Baxtersweb Maps is activated.
* ACF Pro is installed and activated.
* ACF OpenStreetMap Field is installed and activated.
* The required ACF fields have been created.
* Your content contains valid route points or points of interest.

If you're using the shortcode inside a loop, make sure the correct post ID is being passed.

### The map fields don't appear when editing content

Check that your ACF Field Group is assigned to the correct content type.

In ACF, review the **Location Rules** and ensure they include the post type you're editing.

### My route isn't displayed

Verify that:

* At least two valid route points have been added.
* Each route point has a valid map location.
* A routing API key has been entered if automatic route calculation is enabled.

### Points of interest aren't visible

Confirm that:

* Points of interest have been added.
* Each point includes a valid location.
* The map is zoomed appropriately to include all locations.

### Route calculation isn't working

If automatic route calculation fails:

* Confirm that your routing API key has been entered correctly.
* Verify that the API key is still active.
* Check that your routing provider has not exceeded its usage limits.
* Ensure your web server can make outgoing HTTPS requests.

### The map looks incorrect

If markers or routes don't appear as expected:

* Clear your website cache.
* Clear any browser cache.
* Refresh the page.
* Save the plugin settings again.

### JavaScript errors

If the browser console reports JavaScript errors:

* Temporarily disable other plugins to identify conflicts.
* Switch to a default WordPress theme for testing.
* Check whether another plugin is loading incompatible JavaScript.

### I changed the settings but nothing happened

After changing plugin settings:

* Click **Save Changes**.
* Refresh the page.
* Clear any caching plugins.
* Clear your browser cache if necessary.

### I still need help

If the problem persists:

* Review the documentation.
* Visit the Baxtersweb Maps demo.
* Contact Baxtersweb support.

When requesting support, include:

* Your WordPress version.
* Your PHP version.
* Your Baxtersweb Maps version.
* Any error messages.
* The steps required to reproduce the issue.
