### Xweather

Global weather API from Xweather (formerly AerisWeather, now a Vaisala brand), bundling standard weather data with exclusive datasets — global lightning from Vaisala's detection network, a proprietary hail forecast, and road weather — behind a single self-serve interface.

- **Based in:** Eden Prairie (Minneapolis area), Minnesota, USA — the former AerisWeather team; parent company Vaisala is based in Vantaa, Finland
- **Access model:** Instant self-serve — 30-day free trial (free developer account, no credit card) and the published $300/mo plan are both self-serve sign-ups; higher volumes / other plans require sales contact
- **Pricing model:** Paid (30-day free trial, no ongoing free tier)
- **Coverage / data types:** current conditions, observations, forecasts, historical, alerts, severe weather (storm cells/reports, threats, tropical cyclones), air quality, wildfires & fire outlooks, maritime, tides, earthquakes, climate normals, daily records, drought monitor, health/outdoor indices, sun & moon; plus exclusive datasets — global lightning, hail forecast/threats, and road weather; raster map tiles and MapsGL vector map layers also included
- **Free tier:** none ongoing — 30-day trial only (1,000 calls/day, full endpoint access)
- **Paid tiers:** Weather API & Maps — starts at $300/mo (1,000,000 accesses/month, 500 accesses/minute max, Basic support included); higher volumes custom / contact for pricing. Optional paid support add-ons: Essential $50/mo, Business $500/mo (priority response, SLAs)
- **Rate limits:** $300 plan capped at 500 accesses/minute and 1,000,000 accesses/month; trial 1,000 calls/day. Premium datasets consume "access multipliers" (one call counts as multiple accesses)
- **Output formats:** JSON, GeoJSON, CSV, TSV
- **Geographic strength:** global; road weather is limited to the US, Southern Canada, Europe, and Japan
- **Notable limitations:** no ongoing free tier (30-day trial only); one published self-serve paid tier — anything larger or custom needs sales contact; access multipliers on premium datasets make quota estimation less predictable; support beyond Basic is a paid add-on
- **Built on:** blends global/regional sources (NOAA, UK Met Office, DWD, JMA, AirNow, Copernicus, and others) with Xweather's proprietary Xcast AI modeling; lightning comes from Vaisala's proprietary global lightning detection network
- **Docs:** https://www.xweather.com/docs/weather-api
- **Last verified:** 2026-06
