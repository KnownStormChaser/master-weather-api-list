### Foreca

Global weather API from Finnish forecaster Foreca, bundling point forecasts, weather maps, and air quality in its standard package, with marine, warnings, pollen, hurricane, climate, history, and more unlocked on higher tiers or as paid add-ons.

- **Based in:** Espoo, Finland
- **Access model:** Self-serve 30-day free trial (signup form); four tiers (Stratus–Cirrus) carry public list pricing, while the top Nimbus tier is contact-sales. Paid plans are a minimum 12-month term, billed annually
- **Pricing model:** Paid (30-day free trial, no ongoing free tier)
- **Coverage / data types:** point forecasts (current, minutely/15-min nowcast, hourly to 7 days, 3-hourly & daily to 14 days), observations, weather map tiles (radar, satellite, precipitation, temperature, wind, pressure, AQI, snow, pollen), air quality (EPA-standard AQI), marine (waves, sea temperature), pollen (Europe), climate normals (1991–2020), weather history (from Jan 2009), governmental severe-weather warnings (~65 countries), hurricane, plus ski-resort, agriculture, and notification add-ons
- **Free tier:** none ongoing — 30-day trial only (2,000 requests/day, split as 1,000 Point Forecast + 1,000 Map, metered separately)
- **Paid tiers (per month, billed annually):** Stratus €99 (1M req/mo; point forecast + maps + air quality; QPS 10); Cumulus €159 (2M; +marine; QPS 10); AltoCumulus €319 (5M; +marine, 99.5% SLA; QPS 10); Cirrus €449 (10M; +marine/warnings/pollen/hurricane/climate, 99.5% SLA; QPS 50); Nimbus custom / contact sales (custom volume, all features/options, premium support, QPS 500, custom SLAs)
- **Rate limits:** per-tier queries-per-second hard limit (QPS 10 on Stratus–AltoCumulus, 50 on Cirrus, 500 on Nimbus); monthly request cap is a soft limit; limits are per-account (all endpoints aggregate)
- **Output formats:** JSON for data endpoints; map tiles as 256×256 PNG (wind layer as SVG)
- **Geographic strength:** global point forecasts; especially strong European radar/map coverage (plus regional radars for North America, parts of Asia, Australia, and others); pollen is Europe-only
- **Notable limitations:** no ongoing free tier (30-day trial only); paid plans require a 12-month minimum, billed annually; many data types are package- or option-gated (marine from Cumulus up; warnings/pollen/hurricane/climate only on Cirrus+; history, notifications, ski, and agriculture are paid add-ons); pricing is in EUR; Nimbus pricing isn't public; attribution required (must display the Foreca logo or name, plus third-party source attributions on certain layers — e.g. Copernicus CAMS, national met services, EUMETSAT/NOAA)
- **Docs:** https://developer.foreca.com/
- **Last verified:** 2026-06
