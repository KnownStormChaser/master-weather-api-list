### Infoplaza

Developer platform from Dutch weather company Infoplaza, offering a clean global forecast API (current conditions, minutely precipitation, 7-day hourly, 15-day daily) plus a monthly climate API — with a self-serve free Hobby plan and contact-sales pricing above it.

- **Based in:** Houten, Utrecht, Netherlands
- **Access model:** Mixed — the free **Hobby** plan is instant self-serve (register, generate a token); the **Premium/Basic** and **Enterprise** plans are sales contact ("Contact us" — no published prices)
- **Pricing model:** Freemium (ongoing free Hobby tier; paid plans custom / contact for pricing)
- **Coverage / data types:** Weather Forecast API — current conditions, minute-by-minute precipitation (next 2 hours), 7-day hourly forecast, and 15-day daily forecast (temperature, apparent temperature, precipitation type/intensity/probability, wind speed/gust/bearing, humidity, dew point, pressure, cloud cover, visibility, UV index, nearest-storm distance/bearing); plus a separate Weather Climate API for monthly climate data (average temperatures, precipitation patterns, long-term trends)
- **Free tier:** ongoing — Hobby plan: 1,000 requests/month, 1 team member, multiple API keys, analytics
- **Paid tiers:** Premium/Basic (100,000 requests/month, flexible request limit, multiple API keys, unlimited team members, analytics) and Enterprise (unlimited requests, unlimited team members, advanced analytics, custom APIs, SLA) — both custom / contact for pricing
- **Rate limits:** 100 requests/minute (throttled with an error response beyond that); higher limits via contact/upgrade. Plan request quotas are monthly (1,000/mo Hobby, 100,000/mo Premium, unlimited Enterprise)
- **Output formats:** JSON
- **Geographic strength:** global point forecasts by latitude/longitude; Infoplaza is a European (Netherlands-based) operator
- **Notable limitations:** paid pricing isn't public (Premium and Enterprise are contact-sales); the forecast API is queried by lat/lon only (token passed as a query parameter); response keys aren't guaranteed present (the docs advise checking for missing keys); the developer platform currently exposes two APIs (Forecast and Climate) rather than a broad product suite; no severe-weather-alerts or historical-archive endpoint published on the developer platform
- **Docs:** https://developer.infoplaza.com/docs/weather/forecast
- **Last verified:** 2026-06
