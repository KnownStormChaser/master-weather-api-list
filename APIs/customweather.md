### CustomWeather

Global weather data APIs from CustomWeather, a long-running San Francisco–area forecaster, anchored by the self-serve Weather Essentials API — current conditions through 30-day outlooks, marine, severe weather, and optional map tiles — with separate sales-quoted CWS gridded, Maps, Maptiles, and Historical APIs.

- **Based in:** Mill Valley, California, USA
- **Access model:** Mixed — the Weather Essentials API's published Silver/Gold tiers (up to 10M calls/mo) are instant self-serve (subscribe and pay online); the "over 10M calls/mo" tier and the other APIs (CWS, Maps, Maptiles, Historical) are sales contact / request pricing. A 30-day free trial is available via a request form
- **Pricing model:** Paid (30-day free trial, no ongoing free tier)
- **Coverage / data types:** current conditions, detailed 48-hour forecast, hourly (2-day & 7-day) and daily (7/15/30-day) forecasts, astronomy, CustomWeather advisories, US & Canada severe weather, marine (5-day & extended), forecasted airport delays, fire danger; hyperlocal CW100 forecasts to 100 m; 50+ years historical/climate (add-on); plus Gold-tier map-tile layers — global satellite, doppler radar (USA/Canada/Australia), tropical storm paths (global), NWS alerts (USA only), earthquakes, and global contour maps (temperature, dew point, humidity, rainfall, snowfall, ice, wind); CWS gridded/nowcast (HRRR 3 km, 200+ variables) sold separately
- **Free tier:** none ongoing — 30-day trial only (up to 50,000 calls)
- **Paid tiers (Weather Essentials, USD/month):** sold as Silver (no map tiles) / Gold (with map tiles) at each volume — up to 2M calls: Silver $199 / Gold $249; up to 5M: $399 / $499; up to 10M: $749 / $999. Over-10M, plus the CWS, Maps, Maptiles, and Historical APIs: custom / request pricing
- **Rate limits:** monthly call-volume tiers (2M / 5M / 10M+); overage billed at $0.15 CPM (cost-per-thousand); no published per-minute limit. One API request = one location/product combination (bundling multiple products multiplies the billed requests)
- **Output formats:** JSON and XML (metric default; imperial via `metric=false`)
- **Geographic strength:** global, with up-to-100 m hyperlocal resolution and deep US/Canada coverage; some layers are region-bound (doppler radar USA/Canada/Australia, NWS alerts USA only)
- **Notable limitations:** no ongoing free tier (trial only); map tiles, satellite, radar, contour maps, alerts, and earthquakes require the Gold tier; the over-10M tier and the CWS, Maps, Maptiles, and Historical APIs need sales contact / request pricing; historical data is added to a subscription by request; severe weather is US & Canada (NWS alerts US-only); per-request billing is per location/product combination; products are intended to be private-labelled to client branding
- **Built on:** CustomWeather's proprietary "model of models" — the physics-based CW100 hyperlocal model and a 15-day MOS statistical system layered over government NWP (e.g. HRRR for North American nowcasting) and NMME for long-range outlooks, blended with AI/ML, satellite-derived gridded data, and in-house meteorologist input
- **Docs:** https://customweather.com/weather-api-doc/
- **Last verified:** 2026-06
