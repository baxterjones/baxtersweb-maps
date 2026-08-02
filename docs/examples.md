---
description: Practical map structures for common WordPress projects.
icon: book-sparkles
---

# Examples

The same two data types cover most projects: ordered **Map Markers** form the journey, while independent **Points of Interest** add useful context.

## Travel itinerary

Add each destination as a route marker in travel order. Use POIs for hotels, attractions, restaurants or optional stops.

```text
[bxtr_map]
```

## Hiking or cycling trail

Use route markers for the start, checkpoints and finish. Add parking, water points, viewpoints or emergency facilities as POIs.

Road-following routing uses the drivable route returned by openrouteservice, so it may not suit every unmapped footpath or specialist trail. For those maps, the straight-line fallback may be more honest unless the available routing data matches the journey.

## Event or campus map

Use POIs for entrances, stages, parking, toilets, food areas or buildings. Hide the route when there is no intended sequence.

```text
[bxtr_map route="no" poi="yes"]
```

## Delivery or service route

Add scheduled stops as route markers. Use an API key when a road-following overview is useful, while remembering that the map displays a route rather than turn-by-turn navigation.

## Resort or tourism guide

Use a small route for a suggested itinerary and POIs for accommodation, facilities and attractions. Enable POI grouping when many locations occupy the same area.

## Route without supporting places

```text
[bxtr_map route="yes" poi="no"]
```

## Reusable map stored on another post

Keep map data on one content item and display it elsewhere with its post ID:

```text
[bxtr_map id="123"]
```

See the [live demo](https://baxtersweb.com/baxtersweb-maps-demo/) for rendered examples.
