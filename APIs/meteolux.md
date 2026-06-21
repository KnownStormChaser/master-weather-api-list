### MeteoLux

Free, public weather API from MeteoLux — the official meteorological service of Luxembourg, operated by the Administration de la navigation aérienne (ANA) — providing forecasts, current conditions, and official weather warnings (vigilances) for Luxembourg in multiple languages. No API key.

- **Based in:** Findel, Luxembourg (Luxembourg Airport; MeteoLux is the meteorological service of the Administration de la navigation aérienne, ANA)
- **Access model:** No key required — public HTTPS REST endpoints with interactive OpenAPI/Swagger documentation; queried by coordinates. GET only
- **Pricing model:** Free (open public-service data; no fees and no paid tiers)
- **Coverage / data types:** current conditions, 5-day forecasts (daily plus sub-daily 6-hourly steps), and official weather warnings/vigilances (multilingual — English, French, German, and Luxembourgish); forecast parameters include weather condition, temperature, precipitation amount, wind, UV index, and sun & moon / sunshine duration. Reverse geocoding (coordinates → nearest location) is included. The dataset is forecast- and warning-focused: no humidity, dew point, pressure, cloud cover, precipitation probability, air quality, pollen, nowcast, or historical-archive endpoints are exposed
- **Free tier:** the entire API is free; no published per-key quota (no key is used)
- **Paid tiers:** none — there is no commercial or higher-service tier
- **Rate limits:** none published (fair use)
- **Output formats:** JSON (REST API documented via an OpenAPI/Swagger schema at `/api/v1/docs`)
- **Geographic strength:** Luxembourg only — a small, single-country domain centred on the Grand Duchy (observations from the Luxembourg-Findel station)
- **Notable limitations:** Luxembourg-only coverage (single-country); a deliberately narrow parameter set (forecast, current, warnings — no humidity/pressure/cloud/visibility, no precipitation probability, no air quality or pollen, no nowcast, and no observation-history archive exposed in the API); sub-daily forecasts come in 6-hour steps rather than true hourly; lookup is by coordinates with reverse geocoding but no place-name search; data-reuse/licensing terms aren't stated in the API documentation itself — check MeteoLux's legal terms ("Aspects légaux") and attribute MeteoLux as the source; the interactive Swagger page is the primary reference (no separate prose developer guide)
- **Built on:** MeteoLux's own forecaster-analysed forecasts and the Luxembourg-Findel observation station; the underlying NWP model(s) are not enumerated in the API documentation
- **Docs:** https://metapi.ana.lu/api/v1/docs
- **Last verified:** 2026-06
