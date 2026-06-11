### MET Norway (Yr)

Free, public weather API from the Norwegian Meteorological Institute — the data behind Yr — offering global point forecasts plus Nordic nowcasts, marine, alerts, and astronomical data. No API key; just a required identifying User-Agent.

- **Based in:** Oslo, Norway
- **Access model:** No key required — public HTTPS endpoints, but a descriptive User-Agent header with contact info is mandatory (a generic or missing one gets you throttled or blocked); GET only
- **Pricing model:** Free (non-commercial public service funded by Norwegian taxpayers; approved as a UN-recognized Digital Public Good — no paid tiers exist)
- **Coverage / data types:** global point forecasts (Locationforecast — temperature, precipitation, wind, pressure, humidity, cloud cover, weather symbols), precipitation nowcast (Nordic), ocean/marine forecasts (waves, currents, sea temperature), sunrise/sunset & moon (Sunrise/celestial), weather warnings/alerts for Norway (MetAlerts, CAP), subseasonal forecasts, and WMS map layers
- **Free tier:** the entire API is free; no per-key quota is published, but fair-use traffic limits are enforced and clients must identify themselves and cache responsibly
- **Paid tiers:** none — there is no commercial or higher-service tier; high-volume users are asked to run a caching proxy rather than pay
- **Rate limits:** no published hard quota; throttling/blocking is traffic- and User-Agent-based. Clients are expected to honor caching headers (e.g. `If-Modified-Since`) and truncate coordinates to 4 decimals to aid caching; excessive traffic leads to 429/403 and possible bans
- **Output formats:** JSON / GeoJSON (some products also XML); CAP for alerts; gridded data (GRIB/NetCDF) available via THREDDS
- **Geographic strength:** global coverage, but strongest for Norway, the Nordic countries, and the Arctic (local observations + high-resolution post-processing); elsewhere it is ECMWF output interpolated to the point
- **Notable limitations:** mandatory identifying User-Agent (with contact info); no SLA, paid priority, or commercial support; HTTPS/GET only; no `Accept`-header content negotiation (format is chosen via the URL); global forecasts get only minimal post-processing (interpolation + temperature height adjustment), with full treatment reserved for the Nordic/Arctic area; data is licensed under CC BY 4.0 and NLOD, so attribution to MET Norway is required
- **Built on:** ECMWF HRES for global forecasts; the Nordic region and Arctic use MET Norway's own MEPS (MetCoOp Ensemble Prediction System, 2.5 km) and AROME-Arctic models with local-observation post-processing
- **Docs:** https://docs.api.met.no/
- **Last verified:** 2026-06
