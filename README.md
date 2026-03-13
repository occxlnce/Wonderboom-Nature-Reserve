# Wonderboom Nature Reserve Website

Single-page promotional website for Wonderboom Nature Reserve.

## Overview

This project is a static landing page built in plain HTML, CSS, and JavaScript. It combines:

- branded reserve storytelling
- trail and visitor information
- a live weather section powered by Open-Meteo
- local image assets for reserve-specific visuals

The site is designed to run without a build step.

## Project Structure

- `index.html` - the full website, including layout, styles, and scripts
- `img/` - local content images used across the page
- `wblogo.png` - local logo asset
- `wblogo icon.png` - local favicon-style asset

## Features

- custom hero, gallery, trail, weather, pricing, and footer sections
- scroll-based animations and interactive visual effects
- live weather integration for Wonderboom Nature Reserve
- responsive layout for desktop and mobile
- local reserve imagery mapped to relevant sections

## Weather Integration

The weather section fetches live forecast data from [Open-Meteo](https://open-meteo.com/en/docs).

It currently loads:

- current temperature and conditions
- humidity, wind, and rain chance
- sunrise and sunset
- 7-day forecast
- hourly outlook

The weather script refreshes automatically every 30 minutes in the browser.

## Running The Site

Because this is a static site, you can open `index.html` directly in a browser.

For a smoother local workflow, you can also serve the folder with a simple static server.

Examples:

```powershell
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Editing Notes

- Most of the project lives in `index.html`.
- Logos and favicon are currently loaded from Cloudinary URLs in the document head and brand sections.
- Content images are loaded from the local `img/` folder.
- If you change section markup that is referenced in the script, update the related JavaScript selectors too.

## Main External Dependencies

Loaded via CDN:

- Tailwind CSS
- Lucide icons
- Google Fonts

## Next Improvements

- split the page into reusable partials or components
- move styles and scripts into separate files
- add accessibility review and polish
- connect booking/contact CTAs to real actions
- add stronger content management for reserve updates
