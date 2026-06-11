### Open-Meteo

Open-source weather API that aggregates 30+ national weather-service models behind one free, no-sign-up JSON interface, with a free non-commercial tier and paid commercial plans on a dedicated endpoint.

- **Based in:** Bürglen, Switzerland
- **Access model:** Mixed — free non-commercial tier needs no API key (public endpoint, no sign-up, rate-limited); commercial plans are instant self-serve via Stripe checkout (API key for the dedicated customer endpoint); custom/enterprise volume via contact
- **Pricing model:** Freemium (free non-commercial open-access tier; paid commercial plans, Enterprise custom)
- **Coverage / data types:** up-to-16-day forecasts (temperature, precipitation, wind at multiple heights, solar radiation, soil, pressure levels), historical/reanalysis (ERA5 back to 1940) plus historical-forecast/previous-runs/single-runs archives, ensemble, climate projections (CMIP6 to 2050), seasonal (ECMWF SEAS5/EC46), marine waves, air quality (CAMS, incl. pollen), flood (GloFAS river discharge), satellite radiation, geocoding, and elevation
- **Free tier:** non-commercial only — no key, no sign-up; 10,000 calls/day (also 600/min, 5,000/hour, 300,000/month); includes the advanced data APIs (historical, climate, ensemble, seasonal, satellite radiation); no uptime guarantee
- **Paid tiers:** flat monthly subscription on a dedicated endpoint (no per-call overages) — Standard (1M calls/mo, commercial licence, reserved servers; note: omits the advanced data APIs), Professional (5M calls/mo, adds historical/climate/ensemble/seasonal/satellite radiation back), Enterprise (50M+ calls/mo, custom solutions, priority support); billions-scale workloads point to self-hosting
- **Rate limits:** free tier 600/min, 5,000/hour, 10,000/day, 300,000/month; paid plans drop the per-minute/hour/day caps and meter a monthly budget. "API calls" use fractional accounting — requests over 10 variables or beyond ~2 weeks for a single location count as multiple calls
- **Output formats:** JSON (default), CSV, and XLSX (FlatBuffers available for high-performance use); multiple locations per request via comma-separated coordinates
- **Geographic strength:** global; the `best_match` option auto-selects the highest-resolution model per location (1–2 km mesoscale in Central Europe, France, Switzerland, the UK, and North America; 9–11 km global elsewhere)
- **Notable limitations:** the free tier is strictly non-commercial — commercial use requires a paid plan, and CC BY 4.0 attribution is required either way; free tier has no uptime guarantee; the Standard plan notably omits the advanced data APIs (those need the free tier or Professional+); fractional "API call" accounting can multiply usage for wide/long queries; monthly limits are currently soft (email alerts at 80/90/100%, no hard cutoff yet)
- **Built on:** 30+ NWP models from 15+ national services — ECMWF (incl. IFS, ERA5, SEAS5), DWD ICON, NOAA GFS/HRRR, Météo-France ARPEGE/AROME, JMA, KMA, KNMI, DMI, MeteoSwiss, UK Met Office, BOM, CMA, GeoSphere Austria, MET Norway, and GEM (Canada); air quality from Copernicus CAMS, floods from GloFAS, climate from CMIP6, satellite radiation from EUMETSAT/JMA. Server code is open-source (AGPLv3); data is CC BY 4.0
- **Docs:** https://open-meteo.com/en/docs
- **Last verified:** 2026-06
