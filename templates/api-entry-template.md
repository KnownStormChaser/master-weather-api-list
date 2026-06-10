# API entry template

Copy the block below for each new provider. Keep the fields in the same order so entries stay comparable at a glance. Omit any field that genuinely doesn't apply (e.g. leave out **Built on** when the provider doesn't disclose it) rather than writing "unknown".

```markdown
### Provider Name

One-line summary of what the service is and who it's for.

- **Access model:** instant self-serve / paid account / no key required / approval required / sales contact
- **Pricing model:** free / freemium / paid / custom
- **Coverage / data types:** forecast, current, historical, alerts, radar, air quality, marine, etc.
- **Free tier:** specifics, or "none"
- **Paid tiers:** key price points, or "custom / contact for pricing"
- **Rate limits:** if published
- **Output formats:** JSON, CSV, XML, etc.
- **Geographic strength:** where it's strongest / global
- **Notable limitations:** attribution rules, missing data types, SLA caveats, commercial-use restrictions
- **Built on:** underlying model(s) / data source(s) — *only if the provider discloses it*
- **Docs:** link
- **Last verified:** YYYY-MM
```

---

## Field definitions

### Access model — how you get in the door
This is recorded separately from price because it's usually the most decision-relevant detail and changes far less often than dollar figures.

| Value | Meaning |
|---|---|
| **Instant self-serve** | Sign up, get a key, start in minutes. |
| **Paid account, instant** | Self-serve, but behind a paid membership/account. |
| **No key required** | Public endpoint, no signup (may still require an identifying User-Agent). |
| **Approval required** | Application or vetting before access is granted. |
| **Sales contact** | No public signup; you email someone and wait. |

### Pricing model
- **Free** — no cost (note any licensing/attribution requirements).
- **Freemium** — usable free tier plus published paid tiers.
- **Paid** — no usable free tier.
- **Custom / contact for pricing** — usage- or volume-negotiated, or enterprise-only with no public numbers.

### Built on (optional)
Record the underlying model or data feed **only when the provider documents it**. Many APIs don't, blend several sources, or run proprietary models — in those cases leave the field out rather than guessing. Where it maps cleanly to an entry in [master-weather-model-list](https://github.com/KnownStormChaser/master-weather-model-list), a link is a nice touch, but it is not expected for every provider.

### Last verified
Set to the month you confirmed the pricing, free tier, and rate-limit figures against the provider's own documentation. These churn constantly; the date tells a reader how much to trust the numbers.
