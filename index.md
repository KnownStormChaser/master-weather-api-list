# Index

An at-a-glance table of every provider in the catalog. For the full detail on any entry — free-tier specifics, rate limits, output formats, limitations, and what it's built on — open its file in [`APIs/`](./APIs/).

There are no category folders by design; these tables are how you slice the catalog. The list is split into two by **operator type** — independent/commercial providers versus official government and public-service met offices — because that's the most stable dividing line (a national service that later adds a global tier is still government-run, so nothing ever has to be re-filed). To narrow further, use your browser or editor's text search (e.g. `Norway`, `free`, `no key`, `single-country`, `USA`). Pricing and access details change often — each entry file carries its own `Last verified` date.

**A note on the two columns that sound similar.** **Scope** is *what the API returns* — `global`, `multi-country`, or `single-country`. It is not the same as **Geographic strength** (where a provider is most accurate), which lives in the entry files: MET Norway, for example, is global in scope but strongest over the Nordics and Arctic. Scope is kept here as a filterable column rather than as a section, so a coverage change is a one-cell edit and a service that does both can stay in one place.

---

## Commercial & independent providers

| Provider | Based in | Scope | Access | Pricing | Data types |
|---|---|---|---|---|---|
| [AccuWeather](./APIs/accuweather.md) | State College, Pennsylvania, USA | Global | Instant self-serve | Paid | current, forecast, MinuteCast, alerts, imagery |
| [Apple WeatherKit](./APIs/weatherkit.md) | Cupertino, California, USA | Global | Paid account, instant | Paid | current, forecast, alerts, minute precip, historical |
| [CustomWeather](./APIs/customweather.md) | Mill Valley, California, USA | Global | Self-serve / sales contact | Paid | current, forecast, marine, severe, map tiles |
| [Foreca](./APIs/foreca.md) | Espoo, Finland | Global | Free trial / list pricing / sales contact | Paid | forecast, maps, air quality, marine, warnings |
| [Frogcast](./APIs/frogcast.md) | Le Bourget-du-Lac, Savoie, France | Global | Instant self-serve | Paid | forecast, polygon, historical, probabilistic |
| [Infoplaza](./APIs/infoplaza.md) | Houten, Utrecht, Netherlands | Global | Free self-serve / sales contact | Freemium | forecast, minute precip, climate |
| [meteoblue](./APIs/meteoblue.md) | Basel, Switzerland | Global | Free self-serve / sales contact | Freemium | forecast, historical, maps, climate, warnings |
| [Meteomatics](./APIs/meteomatics.md) | St. Gallen, Switzerland | Global | Sales contact (trial available) | Custom | forecast, historical, marine, air quality, climate |
| [Meteosource](./APIs/meteosource.md) | Czech Republic | Global | Instant self-serve / sales contact | Freemium | current, forecast, historical, air quality, maritime |
| [Open-Meteo](./APIs/open-meteo.md) | Bürglen, Switzerland | Global | No key (free) / self-serve (paid) | Freemium | forecast, historical, marine, air quality |
| [OpenWeather](./APIs/openweather.md) | London, UK | Global | Instant self-serve | Freemium | current, forecast, historical, air quality, maps |
| [Pelmorex Weather Source](./APIs/pelmorex-weather-source.md) | Oakville, Ontario, Canada | Global | Free self-serve / sales contact | Freemium | forecast, historical, air quality, alerts, nowcast |
| [Pirate Weather](./APIs/pirate-weather.md) | Ontario, Canada | Global | Instant self-serve | Freemium | forecast, minute precip, alerts (US), historical |
| [Rainbow Weather](./APIs/rainbow-weather.md) | Warsaw, Poland | Global | Instant self-serve | Freemium | precipitation nowcast, map tiles, forecast |
| [The Weather Company](./APIs/the-weather-company.md) | Brookhaven, Georgia, USA | Global | Trial form / Buy now / sales contact | Paid | current, forecast, alerts, historical, imagery |
| [Tomorrow.io](./APIs/tomorrow-io.md) | Boston, Massachusetts, USA | Global | Free self-serve / sales contact | Freemium | real-time, forecast, historical, air quality, alerts |
| [Visual Crossing](./APIs/visual-crossing.md) | Reston, Virginia, USA | Global | Instant self-serve / sales contact | Freemium | current, forecast, historical, maps, air quality |
| [WeatherAPI.com](./APIs/weatherapi.md) | London, UK | Global | Instant self-serve / sales contact | Freemium | realtime, forecast, historical, marine, air quality |
| [Weatherbit](./APIs/weatherbit.md) | Clayton, North Carolina, USA | Global | Instant self-serve / sales contact | Freemium | current, forecast, historical, air quality, lightning |
| [Weatherstack](./APIs/weatherstack.md) | Vienna, Austria | Global | Instant self-serve / sales contact | Freemium | current, forecast, historical, marine, astronomy |
| [Windy API](./APIs/windy.md) | Prague, Czech Republic | Global | Instant self-serve / by agreement | Freemium | point forecast, map tiles, webcams |
| [WorldWeatherOnline](./APIs/worldweatheronline.md) | London, UK | Global | Instant self-serve / sales contact | Freemium | current, forecast, historical, marine, ski |
| [Xweather](./APIs/xweather.md) | Eden Prairie, Minnesota, USA (Vaisala, Finland) | Global | Instant self-serve | Paid | conditions, forecast, lightning, hail, road weather |

---

## Government & public services

Official met offices and public-service providers. Most are free or low-cost, government-funded, and licensed under terms like CC BY / NLOD with attribution required rather than a commercial SLA. Many are **single-country** in scope — this is the section to check first for your country's authoritative API.

| Provider | Based in | Scope | Access | Pricing | Data types |
|---|---|---|---|---|---|
| [MET Norway (Yr)](./APIs/met-norway.md) | Oslo, Norway | Global | No key (User-Agent required) | Free | forecast, nowcast, marine, sunrise/sunset |

*This section is seeded with MET Norway and is where incoming national services — NOAA (USA), Environment and Climate Change Canada, the UK Met Office's public feeds, DWD, Météo-France, and others — will land. Note that several met offices also sell global commercial tiers; they stay here (still government-run), with the commercial product noted in the entry rather than split across both tables.*

---

*Rows in each table are kept alphabetical by provider name (case-insensitive). When adding an entry, drop it into the correct table by operator type and set its `Scope` to what the API actually returns — `global`, `multi-country`, or `single-country` — not where it forecasts best.*
