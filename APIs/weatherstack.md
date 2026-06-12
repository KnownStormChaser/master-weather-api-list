### Weatherstack

Developer-focused REST weather API from apilayer, serving real-time, historical (back to 2008), and forecast data plus marine and astronomy in lightweight JSON — with an ongoing (if very limited) free tier and self-serve paid plans that scale by monthly request volume.

- **Based in:** Vienna, Austria (apilayer Data Products GmbH, registered at the Vienna Commercial Court; part of the US-based Idera, Inc. group, whose legal/imprint address is in Austin, Texas — hence the two locations you'll see cited)
- **Access model:** Instant self-serve — sign up for an API key; the Free, Standard, Professional, and Business plans are all self-serve subscriptions. Enterprise (volume/custom) is sales contact
- **Pricing model:** Freemium (ongoing free tier; self-serve paid tiers; Enterprise custom)
- **Coverage / data types:** current/real-time conditions, hour-by-hour data, historical weather (from 2008), weather forecasts (7-day on Professional, up to 14-day on Business/Enterprise), marine/tide data, astronomy/lunar data, location lookup & autocomplete, and a bulk multi-location endpoint; 40 language options, metric/scientific/imperial units. No severe-weather-alerts, radar, or air-quality endpoints
- **Free tier:** ongoing — 100 calls/month, real-time weather only, HTTPS, no support; non-commercial in practice (commercial use and historical/forecast/marine data require a paid plan)
- **Paid tiers (USD; ~15% off billed yearly):** Standard $9.99/mo (50,000 calls/mo, adds HTTPS, location lookup, astronomy, hour-by-hour, full historical, marine; commercial use); Professional $49.99/mo (300,000 calls/mo, adds 7-day forecast, 40 languages, bulk queries); Business $99.99/mo (1,000,000 calls/mo, 14-day forecast); Enterprise custom / contact for pricing (volume, custom solutions). Over-quota usage is billed per-call as overages rather than cut off
- **Rate limits:** monthly call quotas (100 free → 1M on Business); no published per-minute limit; email/dashboard alerts at 75/90/100%, then per-call overage billing. Errors don't count toward quota
- **Output formats:** JSON (JSONP supported); no XML/CSV
- **Geographic strength:** global, millions of locations; lookup by city name, ZIP, coordinates, or IP
- **Notable limitations:** the free tier is tiny (100 calls/mo, real-time only) and excludes commercial use; HTTPS is gated to paid tiers (free tier is HTTP-only in practice — a security caveat); historical, forecast, marine, astronomy, languages, and bulk queries are all tier-gated; forecast horizon depends on plan (no forecast at all on Free/Standard); no severe-weather alerts, radar, or air-quality data; JSON-only output; support is limited (none on Free, Platinum support only on annual plans)
- **Built on:** weather data licensed from third-party stations and providers rather than a Weatherstack-run model; forecast/marine responses are served via World Weather Online (its icon CDN appears in API output), and the service runs on apilayer's cloud infrastructure
- **Docs:** https://docs.apilayer.com/weatherstack/docs/api-documentation
- **Last verified:** 2026-06
