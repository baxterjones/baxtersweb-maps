---
icon: square-list
---

# Changelog

\= 1.1.11 =

* Updated Name and readme

\= 1.1.10 =

* Fixed per-POI background colours from ACF fields, including shorthand and values entered without a leading hash.
* POI clusters now retain a shared custom colour when all grouped POIs use the same colour.

\= 1.1.9 =

* Existing saved road routes remain available when the API key is removed.
* Maps without saved road geometry are calculated when a valid API key is connected.
* Added routing lifecycle guidance beneath the API key field.
* Fixed the final Plugin Check translator-comment finding.

\= 1.1.7 =

* Fixed global POI background colours on preview and frontend markers.
* Clearing an API key removes cached road geometry and restores fallback lines.
* Route visibility and marker sequence update immediately in the style preview.
* Adjusted marker B's preview popup position.

\= 1.1.6 =

* Retries rural route points with a bounded 2 km road-snapping radius when the default 350 metre search fails.
* Keeps the exact marker location while routing to the nearest mapped drivable road within that limit.

\= 1.1.4 =

* Fixed road-following routes being calculated but not displayed when cached geometry was missing.
* Moved route display and route colour into the Styles tab.
* Renamed Markers & POIs to Styles.
* Improved the admin preview popup position and zoom.

\= 1.1.4 =

* Added a persistent openrouteservice connection status below the API key.
* Replaced the separate save and test controls with Save & Test API.
* Fixed existing maps remaining on dashed fallback lines after connecting the routing API.
* Opens a route marker popup automatically in the admin preview.
* Updated documentation and demo links.
* Improved translation readiness for frontend and admin JavaScript strings.
* Updated external-service documentation for WordPress.org review.

\= 1.0.6 =

* Moved the settings screen under Tools.
* Bundled Leaflet locally instead of loading it from a CDN.
* Replaced POI icon markers with clean text-label markers.
* Added ACF Pro requirement wording.
* Added route marker text colour setting.
* Changed route markers to letter labels.
* Improved duplicate map marker handling.
* Added clearer template and loop shortcode guidance.
* Added Advanced Views Layout shortcode example.
* Added external service disclosure for map tiles and OSRM routing.
* Improved Plugin Check compatibility around nonces, sanitisation, direct file access, and translator comments.

\= 1.0.5 =

* Added map height setting.
* Added border radius setting.
* Added marker label setting with custom label support.

\= 1.0.4 =

* Improved setup experience.
* Added dedicated admin screen.
* Improved generated field layout.
* Improved default map settings.

\= 1.0.3 =

* Prevented duplicate field setup.

\= 1.0.2 =

* Improved onboarding.
* Added uninstall data preference.

\= 1.0.1 =

* Added automated ACF field setup.

\= 1.0.0 =

* Initial release.
