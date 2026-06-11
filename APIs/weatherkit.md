### Apple WeatherKit

Apple's weather API, powered by the Apple Weather service — a native Swift framework on Apple platforms and a REST API everywhere else. Access is bundled into Apple Developer Program membership rather than sold standalone.

- **Based in:** Cupertino, California, USA
- **Access model:** Paid account, instant — requires an Apple Developer Program membership ($99/year USD); once enrolled, you self-serve keys/Service IDs with no separate approval
- **Pricing model:** Paid (membership-gated; 500K calls/month included, no standalone free tier)
- **Coverage / data types:** current conditions, 10-day hourly and daily forecasts (temperature, precipitation, wind, UV index, and more), minute-by-minute precipitation for the next hour (select regions), severe weather alerts (select regions), and historical averages/comparisons
- **Free tier:** none standalone — 500,000 calls/month are included with the $99/year Apple Developer Program membership
- **Paid tiers:** overage subscriptions on top of the included 500K/month, billed monthly in USD: 1M $49.99, 2M $99.99, 5M $249.99, 10M $499.99, 20M $999.99, 50M $2,499.99, 100M $4,999.99, scaling up to 200M $9,999.99
- **Rate limits:** monthly call quota (500K included); no published per-minute limit; unused calls don't roll over, and the quota resets to 0 when a subscription is upgraded
- **Output formats:** JSON (REST API); native Swift framework (WeatherKit) on Apple platforms
- **Geographic strength:** global; minute-by-minute precipitation and severe weather alerts are limited to select regions
- **Notable limitations:** requires Apple Developer Program membership; strict attribution required (must display the Apple Weather "Weather" trademark and a link to other data sources; weather alerts must embed a link to Apple's alert detail page, name the issuing agency, and must not be altered); unused calls don't roll over
- **Built on:** the Apple Weather service — Apple's proprietary global forecast, which blends multiple third-party sources (enumerated in Apple's data-source attribution); successor to the former Dark Sky API
- **Docs:** https://developer.apple.com/documentation/weatherkitrestapi/
- **Last verified:** 2026-06
