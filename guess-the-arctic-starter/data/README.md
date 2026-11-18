# Climate data — placeholder directory

No full CMIP6 arrays are bundled in this starter.

Before adding data exports:
- Source CMIP6 near-surface temperature (`tas`) for CanESM5 r1i1p1f1, historical and SSP1-2.6 / SSP2-4.5 / SSP5-8.5.
- Convert temperatures from Kelvin to Celsius **before** anomaly calculation if needed (the anomaly difference is numerically identical in K and °C).
- Use consistent 1995–2014 baseline, region definitions, area/latitude weighting and temporal averaging.
- Clearly document whether any number is annual, five-year, 10-year, or 2081–2100 average.
- Document how threshold crossings are defined (e.g. first 10-year mean above +3°C).
- Confirm scenario values and figure readings from the original analysis scripts; do not rely on manual transcription alone.
- Do not upload enormous climate binary data files to Git. Keep only lightweight browser-ready JSON/CSV extracts and processing instructions.

Data source: https://console.cloud.google.com/storage/browser/cmip6
