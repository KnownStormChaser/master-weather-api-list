### National Weather Service (NWS)

Free, public weather API from NOAA's National Weather Service — the authoritative US government source for forecasts, severe-weather alerts, and observations across the United States and its territories. No API key; just a required identifying User-Agent.

- **Based in:** Silver Spring, Maryland, USA
- **Access model:** No key required — public HTTPS endpoints; a descriptive User-Agent header identifying your application (ideally with website/email contact info) is mandatory, and NWS notes it may be replaced by an API key in the future. GET only
- **Pricing model:** Free (open US-government data, intended for any use; no fees and no paid tiers)
- **Coverage / data types:** point & gridpoint forecasts (12-hour periods and hourly, ~7 days, on a ~2.5 km grid), raw forecast grid data, current/recent station observations, severe-weather alerts (active plus the past 7 days, in CAP), zone/area forecasts, NWS text products (forecast discussions, etc.), coastal/marine grid forecasts (currently via the raw `forecastGridData` property only), and radar *status* metadata; covers the US, its territories, and adjacent marine zones
- **Free tier:** the entire API is free; no per-key quota is published — a single "reasonable" rate limit applies to everyone (see rate limits)
- **Paid tiers:** none — there is no commercial or higher-service tier
- **Rate limits:** a rate limit is enforced but the exact threshold is **not published**; NWS describes it as generous for typical direct-client use; exceeding it returns an error that usually clears within ~5 seconds; requests routed through shared proxies are far more likely to hit the limit than requests made directly from a client
- **Output formats:** GeoJSON (default, for geometry-bearing endpoints), JSON-LD, DWML (XML, forecast endpoints), OXML (XML observations), CAP (XML, alerts), and ATOM — selected via the `Accept` header
- **Geographic strength:** the United States and its territories only — this is the official US source, with no forecasts outside US jurisdiction
- **Notable limitations:** US (and territories) coverage only — not global; an identifying User-Agent is required (a missing or generic one risks being blocked); the API exposes radar *status* data, **not** radar display imagery (use RIDGE2, the NWS OGC web services, or MRMS for display data); the `/alerts` endpoint only covers the past 7 days (the official archive is via NCEI, not the API); station observations can lag up to ~20 minutes behind real time because of upstream MADIS QC processing; the `gridX`/`gridY` (and occasionally the office) for a coordinate can change, so the `/points` lookup should be re-checked periodically rather than hard-cached forever; HTTPS/GET only
- **Built on:** NWS's own gridded forecasts, produced by each local Weather Forecast Office (WFO) on a ~2.5 km grid (the National Digital Forecast Database lineage); severe-weather alerts issued by WFOs and national centers in CAP; and station observations ingested from MADIS
- **Docs:** https://www.weather.gov/documentation/services-web-api
- **Last verified:** 2026-06
