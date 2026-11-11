# Copenhagen Metro dashboard

A static, interactive overview of Copenhagen's four metro lines (M1–M4), built from a user-provided GTFS timetable snapshot.

**Live dashboard:** [ananya-scripts.github.io/copenhagen-metro-dashboard](https://ananya-scripts.github.io/copenhagen-metro-dashboard/)

## What it shows

- **Network map:** route shapes and stations. Use the M1–M4 buttons above the map to highlight or dim each line; this interaction changes the map only.
- **Scheduled trips by hour:** a stacked chart of trip starts for each line, with the busiest hour called out.
- **Trip mix:** each line's share of scheduled trips in a donut chart.
- **Busiest stations:** the ten stations with the most scheduled stop calls, plus a per-line summary of scheduled trips and stations.
- **Network summary:** scheduled trip and station counts, number of lines, and the timetable's first departure and last arrival.

## Run locally

No build, install, or server is required. Open `index.html` directly in a modern browser:

1. Download or clone this repository.
2. Open `index.html` from the repository folder.

The styles, JavaScript, and derived timetable data are embedded in that file.

## Data and limitations

The embedded data is a Wednesday, **11 November 2026** GTFS service-day snapshot. It contains **2,299 scheduled trips** across M1–M4, with timetable times extending to `24:24` (after midnight on the following calendar day).

This is a static timetable analysis, not a live operations feed. It does not show real-time train locations, delays, passenger counts, or ridership. A station's “scheduled calls” count represents visits by scheduled trains; it is not a measure of how many people use that station. The results describe this particular GTFS snapshot and should not be treated as current service information.

## Deployment

The site is published with GitHub Pages at the live dashboard link above. Because the project is a self-contained static HTML page, it does not require a build step.
