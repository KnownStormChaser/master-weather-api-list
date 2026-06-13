### Meteo.lt (LHMT)

Free, public weather API from the Lithuanian Hydrometeorological Service (Lietuvos hidrometeorologijos tarnyba, LHMT) — Lithuania's official met service, under the Ministry of Environment — providing location forecasts plus meteorological and hydrological station observations for Lithuania. No API key.

- **Based in:** Vilnius, Lithuania
- **Access model:** No key required — public HTTPS REST endpoints queried directly, no signup. GET only
- **Pricing model:** Free (open public-service data; no fees and no paid tiers)
- **Coverage / data types:** location weather forecasts (`long-term` numeric forecast — air & feels-like temperature, wind speed/gust/direction, cloud cover, sea-level pressure, humidity, precipitation, and a weather-condition code; updated ~8×/day, roughly every 3 hours), meteorological station observations (the same parameters plus snow depth, hourly), and hydrological station observations (river/water-body level, water temperature, and discharge). Endpoints are organized around a list of forecast locations, weather stations, and hydro stations
- **Free tier:** the entire API is free; meteorological observations are served for the last 10 years (or from a station's install date if newer); hydrological `measured` data covers the last 30 days, and `historical` hydro data goes back to 2000
- **Paid tiers:** none — there is no commercial or higher-service tier
- **Rate limits:** 180 requests/minute per IP address; LHMT also asks clients not to exceed 20,000 requests/day per IP, warning that doing so can get the IP blocked without notice
- **Output formats:** JSON
- **Geographic strength:** Lithuania only — forecast locations, weather stations, and hydro stations are all within Lithuania
- **Notable limitations:** Lithuania-only coverage (single-country); the official documentation is in Lithuanian only; a single `long-term` forecast type (no nowcast or separate hourly/daily products); no severe-weather-alerts endpoint exposed in the API; observations are per-station and queried by station code and date (no point/lat-lon observation lookup); data is licensed under CC BY-SA 4.0, so attribution to LHMT is required (and the share-alike clause obliges derivatives to use the same licence) — omitting attribution can result in access being cut off; provided "as is" with no quality or fitness guarantees
- **Built on:** LHMT's own numerical weather prediction and its national network of meteorological and hydrological observation stations (specific underlying model not enumerated in the API documentation)
- **Docs:** https://api.meteo.lt/
- **Last verified:** 2026-06
