### OpenWeather

Long-running, developer-focused weather platform from London-based OpenWeather (formerly OpenWeatherMap), with an ongoing free tier, a pay-per-call One Call API, tiered professional subscriptions, and a wide catalog of specialized data products.

- **Based in:** London, UK (additional offices in Paphos, Cyprus and Lewes, Delaware, USA)
- **Access model:** Instant self-serve (sign up, get an API key); free tier, the pay-per-call One Call API, and the four professional subscription tiers are all self-serve. OpenWeather Enterprise is a separate contract-based service via sales contact
- **Pricing model:** Freemium (ongoing free tier, including a student plan; paid pay-per-call and subscription tiers above it)
- **Coverage / data types:** current weather, minutely/hourly/daily forecasts (One Call 4.0 timeline in 1-min, 15-min, 1-hour, 1-day steps), 3-hour/5-day, hourly 4-day, daily 16- and 30-day forecasts, government weather alerts, historical (Time Machine + bulk archives back to 1979), air pollution, weather map layers (current + history/forecast), geocoding, plus specialized products — road risk, solar irradiance/energy, wind, fire weather index, statistical/climate data, accumulated parameters, precipitation maps, and agriculture (AgroMonitoring)
- **Free tier:** ongoing — 60 calls/min, 1,000,000 calls/month (current weather, 3-hour/5-day forecast, air pollution, weather maps, geocoding). A separate **student plan** keeps the same limits and adds history, statistical data, accumulated parameters, hourly 4-day, and daily 16-day. One Call 4.0: first 1,000 calls/day free, then pay-per-call
- **Paid tiers:** One Call 4.0 pay-per-call (beyond the 1,000 free/day); Professional Collection subscriptions — Startup (600 calls/min, 10M/mo), Developer (3,000/min, 100M/mo), Professional (30,000/min, 1B/mo), Expert (100,000/min, 3B/mo), with published monthly pricing and progressively more products/SLA; many specialized APIs priced à la carte (pay-per-call, per month, or per location); Enterprise custom / contact for pricing
- **Rate limits:** free 60 calls/min & 1M/month; One Call 1,000 free calls/day then pay-per-call; subscription tiers from 600/min (Startup) up to 100,000/min (Expert)
- **Output formats:** JSON (default), XML on some core endpoints; weather maps as PNG tiles; bulk archives in CSV and JSON
- **Geographic strength:** global
- **Notable limitations:** standard data is licensed under ODbL (Open Database License), which carries attribution/share-alike obligations; the lineup is fragmented across the free tier, pay-per-call One Call, professional subscriptions, and separately-priced specialty products, which can be confusing; the free tier is limited to basic products (longer forecasts, history, and statistics need the student plan or a paid tier); the student plan requires eligibility verification; some specialty products (e.g. precipitation maps, solar-panel prediction, certain bulks) are contact-sales; higher availability SLAs only apply to higher tiers
- **Built on:** global NWP models (GFS, ECMWF) plus OpenWeather's proprietary hyperlocal model (OWML™/OWHL™), combined via multi-model fusion with weather-station, satellite, and radar data and AI/ML; partnerships with the UK Met Office and other national meteorological agencies
- **Docs:** https://openweathermap.org/api
- **Last verified:** 2026-06
