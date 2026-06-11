### Rainbow Weather

Real-time precipitation specialist from Rainbow Weather (Rainbow.ai), delivering global minute-by-minute precipitation nowcasts (0–4 hours), CDN-served map tiles, and hourly/daily weather through self-serve REST APIs with free tiers and pay-as-you-go pricing.

- **Based in:** Warsaw, Poland
- **Access model:** Instant self-serve — sign up, get an API key, and start; a free tier is included and usage beyond it is pay-as-you-go (no sales contact required for the published products)
- **Pricing model:** Freemium (per-product monthly free allotments plus pay-as-you-go per-unit pricing)
- **Coverage / data types:** Precipitation Nowcast API (REST/JSON) — minute-by-minute precipitation up to 4 hours ahead, globally, by lon/lat, returning precip rate (mm/h), type (rain/snow/mixed/none), and a max-intensity summary; 1-minute resolution, ~10-minute update cadence (separate local and global endpoints). Map Tiles API (XYZ/CDN) — global cloud-cover and precipitation-nowcast raster tiles (256×256 px) from radar + satellite fusion, compatible with Leaflet, Mapbox GL, deck.gl, and any XYZ tile SDK; ~10-minute cadence. Weather API (REST/JSON) — hourly and daily forecasts by lon/lat (temperature, precipitation, wind, pressure, humidity, UV index, visibility, dew point, etc.), 1-hour resolution
- **Free tier:** ongoing — per-product monthly allotments: Nowcast 5,000 requests/mo; Weather 5,000 requests/mo; Map Tiles 30,000 tiles/mo
- **Paid tiers:** pay-as-you-go beyond the free allotments — Nowcast $0.10 / 1K requests; Weather $0.10 / 1K requests; Map Tiles $0.20 / 1K tiles (no fixed subscription tiers published)
- **Rate limits:** no published per-minute limit; metered by monthly request/tile volume against the free allotment, then per-unit pricing; data is CDN-delivered and refreshed roughly every 10 minutes
- **Output formats:** JSON (Nowcast and Weather APIs); 256×256 px raster tiles via XYZ/CDN (Map Tiles)
- **Geographic strength:** global; the high-resolution local nowcast endpoint may return 404 where radar/coverage is unavailable, while a separate precip-global endpoint covers worldwide
- **Notable limitations:** a focused, young product — its core strength is short-range precipitation nowcasting (0–4 h) rather than medium-range forecasting; the Weather API is hourly/daily and relatively new ("more weather parameters coming soon"); no historical archive, severe-weather alerts, or air-quality endpoints; pay-as-you-go per-unit billing only (no flat subscription tiers); the nowcast `start_timestamp` can only be set within the past 30 minutes
- **Built on:** a fused radar + satellite machine-learning pipeline that produces the precipitation nowcasts, with precipitation-type classification and intensity scoring
- **Docs:** https://doc.rainbow.ai/
- **Last verified:** 2026-06
