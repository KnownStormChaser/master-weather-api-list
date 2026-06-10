# master-weather-api-list

This repository is a **simple, human-readable catalog of weather forecast APIs** — the services developers use to pull forecasts, current conditions, alerts, and related data into their own applications.

Where its companion project [master-weather-model-list](https://github.com/KnownStormChaser/master-weather-model-list) documents the raw forecast models and the satellite data that feeds them, this repository documents the **services built on top of that layer** — including commercial ones. Its focus is breadth: not just the handful of providers that dominate every "best weather API" list, but the **independent alternatives** and the **national and regional meteorological services** for people who want to keep things local rather than defaulting to the usual American options.

No meteorology or backend background is required to use this repository.

The goal is to make it easy to discover:
- which weather APIs exist
- who runs them
- what data they provide
- how you actually get access (and at what cost)
- and which ones are worth a look beyond the obvious few

---

## What this repository includes
- **Commercial and paid APIs.** Unlike the model catalog, paid providers belong here — selling forecast access is how most of these services operate. Pricing is recorded as a clearly-labelled field, not used to exclude.
- **Free and freemium APIs**, including those with no-signup public endpoints and those with a usable free tier
- **Independent and lesser-known providers** that rarely appear in "top weather API" listicles
- **National and regional meteorological service APIs** (official met offices and public-service providers)
- **Forecast-focused services** — current conditions, hourly/daily forecasts, and severe weather alerts — with each entry noting the other data types it bundles (radar, air quality, marine, historical, etc.)
- For each provider, **how access actually works** — instant self-serve key, paid account, no key required, approval gate, or sales contact — recorded separately from price, since that's the most stable and decision-relevant detail
- Where the provider discloses it, **what the API is built on** (an underlying model or data feed). Many providers don't publish this, and some run proprietary models — so this is an optional field, filled in only when it's genuinely known

---

## What this repository does NOT include
- Consumer weather apps and websites that don't expose a developer API
- Pure map-tile or radar-viewer products with no queryable data API (may be added later)
- Retired or discontinued APIs (except where noted for historical context)
- For now, **archive/historical-only or radar-only services** — point and area forecast APIs come first; other categories may follow

A note on commercial APIs: a paywall is a reason to exclude a model from the companion repository, but it is **not** a reason to exclude an API here. Each entry labels its **pricing model** and, separately, its **access model**, so you can tell "sign up and start in minutes" apart from "email sales and wait." That access distinction is often more useful than the dollar figure, and it changes far less often.

A note on the "built on" field: where a provider states which model or data source powers its forecasts, the entry records it. But weather APIs frequently don't disclose this, blend many sources, or run their own proprietary models — so the field is left out rather than guessed at when it isn't clearly documented.

---

## Repository structure

Every provider gets its own file in a single flat [`APIs/`](./APIs/) folder — **one entry per provider**, named predictably (e.g. `accuweather.md`, `open-meteo.md`). There are no sub-folders: not by country, not by commercial-vs-government, and not by data type.

This is deliberate. The obvious category splits all overlap. Several national met offices (the UK Met Office, Météo-France, DWD) also sell commercial API tiers; "independent" providers often have paid plans too; and country folders would scatter the list into a pile of one-entry directories. Forcing each provider into a single bucket would misfile more entries than it would organize. Keeping one entry per provider also matches how these APIs are actually sold — as bundles (one key, one set of docs covering forecasts, alerts, and the rest), not as separable data types.

Browsing by a slice — the non-American ones, the free ones, the national services — is handled by an index rather than by folders:

- [`INDEX.md`](./INDEX.md) — a single scannable table of every provider (name, where it's based, access model, pricing model, coverage), so the whole catalog can be taken in at a glance or narrowed with a quick text search

Each entry describes:
- what the service is and who it's for
- where the provider is based
- what data types it provides
- how you get access, and the pricing model
- free tier, rate limits, and output formats where published
- geographic strengths and notable limitations

New entries should start from the template in [`templates/`](./templates/).

---

## Why this exists

Information about weather APIs is usually one of two things: a paid provider's own marketing, or an SEO listicle that recycles the same five names. Neither helps much if you're trying to compare options fairly, find something cheaper, or use a service local to your region.

This repository aims to provide a **clear, neutral, and beginner-friendly index** of what's available — commercial and free, well-known and obscure, American and otherwise.

---

## Supporting this project

This repository is maintained as independent research. Everything stays free and openly accessible — no paywalls, accounts, ads, or affiliate links.

If you've found the catalog useful in your work or research, you can optionally support ongoing maintenance through any of the following:

- [GitHub Sponsors](https://github.com/sponsors/KnownStormChaser)
- [Ko-fi](https://ko-fi.com/knownstormchaser)
- [Buy Me a Coffee](https://buymeacoffee.com/sebastianpd)
- [Liberapay](https://liberapay.com/KnownStormChaser)

Sponsorship helps support the time this takes: verifying pricing and access details, tracking tier and rate-limit changes, and adding new providers as they appear. Even small contributions are meaningful and appreciated — but the catalog will always be free for everyone.

---

## Disclaimer

This repository is for **information and discovery only**.
Always consult the official provider's documentation for:
- current pricing and quotas
- data usage terms and licensing
- operational or safety-critical use

Nothing here is an endorsement, and no affiliation with any listed provider is implied.

---

## A note on accuracy

I try to document each API as accurately as possible based on official provider documentation. However, **information in this repository may be incomplete, out of date, or inaccurate.** This is especially true for:

- Pricing tiers, free quotas, and rate limits, which change frequently and often without announcement
- Free-tier terms (commercial vs non-commercial use, attribution requirements)
- Data types and endpoints added or removed between documentation updates
- Providers with limited English-language documentation

Pricing and limits change far more often than the underlying models do, so each entry carries a **`Last verified`** date. Treat anything older than a few months as needing a re-check against the provider's own docs.

If you spot an error or know of a change, please see the [Contributions](#contributions) section — corrections are genuinely welcome and are the main way this catalogue stays useful over time.

---

## Contributions

Corrections, additions, and improvements are welcome.

If you add a provider, please ensure:
- pricing, free tier, and rate limits are verified against the provider's own docs, with `Last verified` set to the current month
- links point to official sources
- descriptions remain simple, factual, and non-promotional
- the entry uses the template in [`templates/`](./templates/) as a starting point
