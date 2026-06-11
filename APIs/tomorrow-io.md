### Tomorrow.io

AI-driven weather data API from Tomorrow.io (legal entity The Tomorrow Companies Inc.), with 60+ data layers spanning real-time, forecast, historical, and specialized environmental data — a self-serve free tier, with everything beyond it gated behind Enterprise sales.

- **Based in:** Boston, Massachusetts, USA
- **Access model:** Mixed — Free plan is instant self-serve (sign up, get an API key); the paid Enterprise plan requires sales contact (no published self-serve paid tiers)
- **Pricing model:** Freemium (ongoing free tier; Enterprise custom / contact for pricing)
- **Coverage / data types:** real-time/current conditions, forecasts (5-day on Free, up to 14-day on Enterprise), historical (24 hours on Free, up to ~20 years on Enterprise), 40+ core parameters (temperature, wind, precipitation, humidity, pressure, etc.), severe weather alerts/insights, weather map tiles, location monitoring/alerting, and weather-on-routes; premium layers — air quality, pollen, solar, soil/land, lightning, fire, flood, maritime, aviation (METAR/TAF) — are Enterprise-only
- **Free tier:** real-time + 5-day forecast, core weather layers, 24h historical, 1 monitored location, 1 alert; API-only (no platform UI access)
- **Paid tiers:** Enterprise — custom / contact for pricing (adds 14-day forecast, premium data layers, minutely resolution, advanced historical, weather maps, custom SLAs, SSO, custom monitored locations/alerts)
- **Rate limits:** Free plan 500 requests/day, 25/hour, 3/second, resetting at midnight UTC (no separate monthly cap); Enterprise limits are custom
- **Output formats:** JSON; weather map tiles for interactive map libraries (Mapbox, Google Maps, Leaflet, OpenLayers, Cesium)
- **Geographic strength:** global, hyperlocal high-resolution
- **Notable limitations:** Enterprise pricing isn't public (sales contact required); the free plan is API-only and limited (5-day forecast, 24h history, core layers, 1 monitored location/1 alert); premium layers and the 14-day forecast require Enterprise; commercial/scaling use is routed to sales
- **Built on:** Tomorrow.io's proprietary modeling (including its CBAM model), blending traditional data sources, AI/ML, and data from its own weather-sensing satellite constellation
- **Docs:** https://docs.tomorrow.io/reference/welcome
- **Last verified:** 2026-06
