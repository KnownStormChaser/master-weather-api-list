### Pirate Weather

Open-source, Dark Sky-compatible weather API built directly on public NOAA forecast models — created and run by a single developer (Alexander Rey) as a community project, and a drop-in replacement for the retired Dark Sky API.

- **Based in:** Ontario, Canada
- **Access model:** Instant self-serve — every plan, from Free up through the $350/mo Enterprise tier, is a self-serve subscription via the developer portal (Apiable); custom API keys ($75+ tiers) are arranged by emailing the maintainer
- **Pricing model:** Freemium (ongoing free tier; self-serve paid subscription tiers)
- **Coverage / data types:** Dark Sky-style currently / minutely / hourly / daily (7-day) forecasts — temperature, apparent temperature, precipitation (type, intensity, probability, accumulation), wind, humidity, dew point, pressure, cloud cover, visibility, UV index, ozone, smoke, fire index; weather alerts (US only); historical "time machine" via ERA5 reanalysis; an MCP server is also included on all tiers. Multiple unit systems (us, si, ca, uk2)
- **Free tier:** 10,000 requests/month (personal/non-commercial use); includes the 7-day forecast, historical data, and MCP server
- **Paid tiers (USD/month, all self-serve):** $3 → 20,000 calls/mo; $5 → 60,000 (+testing-backend endpoint); $25 → 325,000; $75 → 1,000,000 (+custom key); $350 "Enterprise" → 5,000,000 (+custom key, setup/implementation support, priority on adding custom variables)
- **Rate limits:** monthly call quota per key (10,000 free → 5M on Enterprise; e.g. ~23 calls/min at 1M, ~100/min at 5M); response headers report remaining quota and reset time; over-quota requests return a 429
- **Output formats:** JSON (Dark Sky-compatible response structure)
- **Geographic strength:** global via NOAA GFS; high-resolution coverage of the US and much of Canada via NBM and HRRR; weather alerts are US-only
- **Notable limitations:** forecasts are raw NOAA model output by design — minimal processing, no proprietary bias correction (a transparency feature, not a flaw); weather alerts are US-only; single-maintainer community project (the $350 tier adds setup support, but it remains a solo-run service rather than a traditional enterprise SLA); historical ERA5 data exposes fewer parameters than the live forecast; minor doc inconsistencies (e.g. the historical range is cited as both 1940 and 1980 across pages)
- **Built on:** public NOAA models pulled from AWS Open Data (via the Herbie package) — NBM (National Blend of Models, primary for the US/Canada), HRRR (US/southern-Canada high-resolution, sub-hourly), GFS (global and beyond 48 h), and GEFS (ensemble, used for precipitation type/probability), with a NBM → HRRR → GEFS → GFS fallback order; ERA5 reanalysis powers the historical endpoint. Every processing step is documented and the server code is open-source
- **Docs:** https://docs.pirateweather.net/
- **Last verified:** 2026-06
