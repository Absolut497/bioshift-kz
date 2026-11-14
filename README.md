# BioShift KZ

**Smart crop rotation and early crop-stress detection using NASA Earth observation data.**
An agricultural decision-support platform for farmers in Kazakhstan, piloted in the Almaty Region (Enbekshikazakh and Ili Districts).

NASA Space Apps Challenge project.

> **Status: prototype with sample data.** The demo page shows how the platform works with illustrative values. Connection to live NASA data is the planned next step.

## Live demo

See the GitHub Pages link in the repository's "About" section.
Presentation: `BioShift_KZ.pdf` in this repository.

## Two stages, one platform

### Land Booster (before planting)
Recommends crop rotation scenarios from multi-year vegetation trends, regional soil moisture, weather history and the farmer's crop history.
Example: *Legume crop → Winter wheat*. Legumes can add soil nitrogen through biological nitrogen fixation. The **WHY?** button lists the factors behind each recommendation.

### Anti-Stress Radar (during growth)
Highlights possible crop-stress zones on a field map (green: no significant anomaly, yellow: possible stress, red: inspection recommended) and helps prioritize inspection and irrigation.

Every recommendation shows the latest observation date, spatial resolution, data availability and a confidence level.

## NASA data

| Dataset | Use |
|---|---|
| MODIS (NDVI) | Multi-year vegetation trends |
| SMAP | Regional soil moisture |
| ECOSTRESS | Plant surface temperature anomalies |
| GPM IMERG | Regional precipitation |
| NASA POWER | Temperature and precipitation history |
| NASA AppEEARS | Data extraction and preparation |

## Technology

- Demo page: HTML, JavaScript, [Leaflet](https://leafletjs.com/), OpenStreetMap tiles
- Planned platform: Python + FastAPI backend, React + Leaflet frontend, Chart.js charts, NASA AppEEARS for data extraction

## Limitations

Satellite data provides estimates, not direct soil laboratory measurements. Field inspection and soil sensors can improve accuracy. BioShift KZ is a decision-support tool, not a replacement for farmers or agronomists.

## Run locally

Open `index.html` in a browser (internet connection needed for map tiles and Leaflet).

## Credits

NASA Earth observation data and services; Leaflet; OpenStreetMap contributors; Inter and Space Grotesk fonts (Google Fonts). Code and text drafted with help from Claude (Anthropic).

## License

MIT
