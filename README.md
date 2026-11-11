# Bank of Russia Exchange Rates API — cbr-exchange-rate

[![npm version](https://img.shields.io/npm/v/cbr-exchange-rate.svg)](https://www.npmjs.com/package/cbr-exchange-rate)
[![license](https://img.shields.io/npm/l/cbr-exchange-rate.svg)](https://github.com/AllRates-Today/cbr-exchange-rate/blob/main/LICENSE)
[![zero dependencies](https://img.shields.io/badge/dependencies-0-brightgreen.svg)](https://www.npmjs.com/package/cbr-exchange-rate)
[![TypeScript](https://img.shields.io/badge/TypeScript-types%20included-3178C6.svg)](https://www.typescriptlang.org/)
[![USD/RUB today](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fallratestoday.com%2Fapi%2Fopen%2Fcentral-bank%2Fcbr%3Fsource%3DUSD%26target%3DRUB&query=%24.rate&label=USD%2FRUB%20official%2C%20Bank%20of%20Russia&color=0A7E8C&cacheSeconds=3600)](https://allratestoday.com/central-bank-rates-api/cbr/)
[![rate date](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fallratestoday.com%2Fapi%2Fopen%2Fcentral-bank%2Fcbr%3Fsource%3DUSD%26target%3DRUB&query=%24.rate_date&label=rate%20date&color=555&cacheSeconds=3600)](https://allratestoday.com/central-bank-rates-api/cbr/)

**Official Bank of Russia (Russia) daily exchange rates for Node.js and TypeScript. The published central bank rates behind tax filings, customs valuations, audits, and compliant invoicing — not market estimates, but the numbers Bank of Russia itself prints, every business day.**

## 🚀 Why this client?

- 🏛️ **Official rates** — Bank of Russia's own table, with the publisher's own `rate_date` on every response
- 📅 **History back to 2016** — point-in-time tables and daily series for any past date
- 🔀 **Official vs derived, always flagged** — computed inverse/cross pairs carry `derived: true`, never mixed with official prints
- ⚡ **Zero dependencies** — pure ESM + CJS over global `fetch`; Node 18+, Bun, Deno, and edge runtimes
- 🔷 **Type-safe** — full TypeScript definitions shipped with the package
- 🧾 **Compliance-grade metadata** — `rate_type`, publication date, and source disclaimer on every response

> **Official rate, not mid-market:** every value here is a number Bank of Russia itself published, fixed once printed and carrying the central bank's own `rate_date` — what filings and audits require. Need the live mid-market rate for pricing or display instead? Use the [mid-market API](https://allratestoday.com/docs/) or [`@allratestoday/sdk`](https://www.npmjs.com/package/@allratestoday/sdk). The two can diverge by several percent.

## 🔑 Get your API key

Get a free API key at [allratestoday.com/register](https://allratestoday.com/register) — no credit card required. Latest rates are on every plan, including free.

## 📈 Latest official table

[![Latest Bank of Russia table](https://allratestoday.com/api/open/central-bank/cbr/table.svg)](https://allratestoday.com/central-bank-rates-api/cbr/)

The image is rendered live from the keyless endpoint, so it follows the central bank's publications on npm and on GitHub alike without a new release. The same table as text is folded below for search and copy-paste: on GitHub [a daily Action](.github/workflows/daily-table.yml) refreshes it whenever the central bank publishes a new table; on npm it is as of the package's publish date.

<!-- daily-table:start -->
<details>
<summary>Table as text: published 2026-11-11 by Bank of Russia — 54 rates. Updated 2026-11-11.</summary>

| Base | Quote | Type | Rate |
| --- | --- | --- | ---: |
| AED | RUB | reference | 22.4775 |
| AMD | RUB | reference | 0.229028 |
| AUD | RUB | reference | 57.1567 |
| AZN | RUB | reference | 48.558 |
| BDT | RUB | reference | 0.661838 |
| BHD | RUB | reference | 219.4967 |
| BOB | RUB | reference | 7.02541 |
| BRL | RUB | reference | 14.9699 |
| BYN | RUB | reference | 27.4988 |
| CAD | RUB | reference | 58.4498 |
| CHF | RUB | reference | 100.5587 |
| CNY | RUB | reference | 12.3845 |
| CUP | RUB | reference | 3.43953 |
| CZK | RUB | reference | 3.79325 |
| DKK | RUB | reference | 12.3604 |
| DZD | RUB | reference | 0.606388 |
| EGP | RUB | reference | 1.54822 |
| ETB | RUB | reference | 0.512732 |
| EUR | RUB | reference | 92.3966 |
| GBP | RUB | reference | 110.6399 |
| GEL | RUB | reference | 31.8192 |
| HKD | RUB | reference | 10.5211 |
| HUF | RUB | reference | 0.255632 |
| IDR | RUB | reference | 0.00455994 |
| INR | RUB | reference | 0.879506 |
| IRR | RUB | reference | 0.0000435142 |
| JPY | RUB | reference | 0.522096 |
| KGS | RUB | reference | 0.943954 |
| KRW | RUB | reference | 0.06089 |
| KZT | RUB | reference | 0.183858 |
| MDL | RUB | reference | 4.60137 |
| MMK | RUB | reference | 0.0393089 |
| MNT | RUB | reference | 0.0229188 |
| NGN | RUB | reference | 0.061177 |
| NOK | RUB | reference | 8.77253 |
| NZD | RUB | reference | 46.4625 |
| OMR | RUB | reference | 214.6908 |
| PLN | RUB | reference | 21.1127 |
| QAR | RUB | reference | 22.6782 |
| RON | RUB | reference | 17.336 |
| RSD | RUB | reference | 0.788149 |
| SAR | RUB | reference | 22.013 |
| SEK | RUB | reference | 8.40275 |
| SGD | RUB | reference | 64.5769 |
| THB | RUB | reference | 2.47211 |
| TJS | RUB | reference | 8.96614 |
| TMT | RUB | reference | 23.5853 |
| TRY | RUB | reference | 1.6466 |
| UAH | RUB | reference | 1.81776 |
| USD | RUB | reference | 82.5486 |
| UZS | RUB | reference | 0.00688243 |
| VND | RUB | reference | 0.00322455 |
| XDR | RUB | reference | 111.8401 |
| ZAR | RUB | reference | 5.04838 |

</details>

Source: [Official rates published by CBR, served by AllRatesToday](https://allratestoday.com/central-bank-rates-api/cbr/). Rates are as printed by the central bank; AllRatesToday is not affiliated with it.
<!-- daily-table:end -->

## 📦 Installation

```bash
npm install cbr-exchange-rate
```

```bash
yarn add cbr-exchange-rate
```

```bash
pnpm add cbr-exchange-rate
```

Requires Node 18+ (global `fetch`); also runs on Bun, Deno and edge runtimes. Also published under the org scope as [`@allratestoday/cbr-exchange-rate`](https://www.npmjs.com/package/@allratestoday/cbr-exchange-rate) — same code, same versions.

## 🏁 Quick start

```js
import { getRate } from 'cbr-exchange-rate';

const pair = await getRate('USD', 'RUB', { apiKey: 'art_live_...' });
console.log(pair.rate, pair.rate_date); // the official Bank of Russia rate, on the central bank's own date
```

## 📚 API reference

- [Latest pair rate](#latest-pair-rate) — one pair from the latest official table
- [Full official table](#full-official-table) — everything the central bank printed, in one call
- [Table for a date](#table-for-a-date) — the official table for an invoice or filing date
- [Daily time series](#daily-time-series) — one pair across a date range

---

### Latest pair rate

Free plan and up. Pairs the central bank does not print directly are resolved from its table and flagged (see *Official vs derived rates* below).

```js
const pair = await getRate('USD', 'RUB', { apiKey: 'art_live_...' });
```

**Response:**

```javascript
{
  bank: 'cbr',
  name: 'Bank of Russia',
  rate_date: '2026-11-11',   // Bank of Russia's own publication date
  source: 'USD',
  target: 'RUB',
  rate: 82.5486,
  rate_type: 'reference',
  derived: false,
  method: 'published',
  disclaimer: 'Official rates as published by the named central bank. On weekends/holidays the most recent published rate_date is returned.'
}
```

### Full official table

Free plan and up. The complete table for the latest publication date.

```js
import { getLatestRates } from 'cbr-exchange-rate';

const table = await getLatestRates({ apiKey: 'art_live_...' });
console.log(table.rate_date, table.rates.length);
```

**Response:**

```javascript
{
  bank: 'cbr',
  name: 'Bank of Russia',
  rate_date: '2026-11-11',
  rates: [
    { "base": "USD", "quote": "RUB", "type": "reference", "value": 82.5486 },
    // … the rest of the official table (54 currencies vs RUB)
  ],
  disclaimer: '…'
}
```

### Table for a date

Paid plans. The official table for any date since 2016 — weekends and holidays return the most recent published date, flagged via `published_on_requested_date`, which is exactly the in-force rate a filing needs.

```js
import { getRatesForDate } from 'cbr-exchange-rate';

const day = await getRatesForDate('2026-06-30', { apiKey: 'art_live_...' });
// Optionally narrow to one pair:
const one = await getRatesForDate('2026-06-30', { apiKey: 'art_live_...', source: 'USD', target: 'RUB' });
```

**Response:**

```javascript
{
  bank: 'cbr',
  requested_date: '2026-06-30',
  rate_date: '2026-06-30',                // the date actually published
  published_on_requested_date: true,      // false when a weekend/holiday fell back
  rates: [ /* the full table for that date */ ],
  disclaimer: '…'
}
```

### Daily time series

Paid plans. One resolved rate per publication date — ready for charting, revaluation runs, or audit workpapers.

```js
import { getHistory } from 'cbr-exchange-rate';

const series = await getHistory(
  { source: 'USD', target: 'RUB', from: '2026-01-01', to: '2026-11-11' },
  { apiKey: 'art_live_...' }
);
```

**Response:**

```javascript
{
  bank: 'cbr',
  source: 'USD',
  target: 'RUB',
  from: '2026-01-01',
  to: '2026-11-11',
  count: 152,
  rates: [
    // one entry per publication date
    { date: '2026-11-11', rate: 82.5486, rate_type: 'reference', derived: false, method: 'published' },
    // …
  ],
  disclaimer: '…'
}
```

Pass `{ symbol: 'USD' }` instead of `source`/`target` to get the raw published rows for one currency (all rate types, no pair resolution).

---

## 🗺️ Currencies covered

Bank of Russia currently publishes rates covering **54 currencies** against the RUB (as of the latest table):

🇦🇪 `AED` · 🇦🇲 `AMD` · 🇦🇺 `AUD` · 🇦🇿 `AZN` · 🇧🇩 `BDT` · 🇧🇭 `BHD` · 🇧🇴 `BOB` · 🇧🇷 `BRL` · 🇧🇾 `BYN` · 🇨🇦 `CAD` · 🇨🇭 `CHF` · 🇨🇳 `CNY` · 🇨🇺 `CUP` · 🇨🇿 `CZK` · 🇩🇰 `DKK` · 🇩🇿 `DZD` · 🇪🇬 `EGP` · 🇪🇹 `ETB` · 🇪🇺 `EUR` · 🇬🇧 `GBP` · 🇬🇪 `GEL` · 🇭🇰 `HKD` · 🇭🇺 `HUF` · 🇮🇩 `IDR` · 🇮🇳 `INR` · 🇮🇷 `IRR` · 🇯🇵 `JPY` · 🇰🇬 `KGS` · 🇰🇷 `KRW` · 🇰🇿 `KZT` · 🇲🇩 `MDL` · 🇲🇲 `MMK` · 🇲🇳 `MNT` · 🇳🇬 `NGN` · 🇳🇴 `NOK` · 🇳🇿 `NZD` · 🇴🇲 `OMR` · 🇵🇱 `PLN` · 🇶🇦 `QAR` · 🇷🇴 `RON` · 🇷🇸 `RSD` · 🇸🇦 `SAR` · 🇸🇪 `SEK` · 🇸🇬 `SGD` · 🇹🇭 `THB` · 🇹🇯 `TJS` · 🇹🇲 `TMT` · 🇹🇷 `TRY` · 🇺🇦 `UAH` · 🇺🇸 `USD` · 🇺🇿 `UZS` · 🇻🇳 `VND` · `XDR` · 🇿🇦 `ZAR`

## 🏛️ Source

The Bank of Russia is the central bank of the Russian Federation. It sets official ruble exchange rates for dozens of currencies once per business day, announced in the afternoon Moscow time and effective for the following calendar day.

- Publisher's own page: [Official exchange rates on selected date](https://www.cbr.ru/eng/currency_base/daily/) · [www.cbr.ru](https://www.cbr.ru)
- Publication: every business day; the exact schedule, freshness status and any current delay are on the [Bank of Russia rates page](https://allratestoday.com/central-bank-rates-api/cbr/)
- In the API: usually by **15:20 UTC** (measured over the last 11 publications). Schedule a sync at or after that time and retry hourly until `rate_date` moves; every response carries the same figure as `available_by_utc` — see [when to poll](https://allratestoday.com/docs/#when-to-poll)
- Values are stored unmodified, with the publisher's own `rate_date` on every row — see the [methodology](https://allratestoday.com/official-rates-methodology/)

## 🧭 Reading the numbers

- `value` is always **quote currency per 1 unit of base currency** (`base: "EUR", quote: "USD", value: 1.15` means 1 EUR = 1.15 USD).
- Bank of Russia quotes **RUB per 1 unit of foreign currency** (e.g. `base: "USD", quote: "RUB"` means RUB per one US dollar).
- Need the other way round? Ask `getRate(target, source)` and the API inverts or crosses for you, flagged `derived: true` — never divide a published rate yourself in a compliance workflow.
- `rate_type` tells you which of the central bank's series a row belongs to (`reference` here); some publishers print buy/sell or several fixings for the same pair.

## 🧩 ERP & accounting systems

Loading the official Bank of Russia rate into an accounting system is a supported workflow, not a hack. Step-by-step guides with the direction each system expects:

- [Dynamics 365 Business Central](https://allratestoday.com/docs/integrations/business-central/) — built-in Currency Exchange Rate Service, no code
- [Xero](https://allratestoday.com/docs/integrations/xero/) · [QuickBooks Online](https://allratestoday.com/docs/integrations/quickbooks/) · [SAP S/4HANA and ECC](https://allratestoday.com/docs/integrations/sap/) · [Odoo](https://allratestoday.com/docs/integrations/odoo/)

The same keyed endpoints return `?format=csv`, `?format=xml` and `?format=xlsx`, and accept the key as `?api_key=` on the URL for importers that cannot send headers:

```bash
curl "https://allratestoday.com/api/v1/central-bank/cbr/latest?format=xml&api_key=art_live_..."
```

## 🤖 AI agents

- MCP server: `npx -y @allratestoday/central-bank-mcp` (stdio) or the hosted endpoint `https://allratestoday.com/api/mcp` — tools for official rates, history, cross-bank comparison and publication calendars
- Already using the general SDK or MCP server? Since 2026-10-01 [`@allratestoday/sdk`](https://www.npmjs.com/package/@allratestoday/sdk) 1.4+ has `officialRates('cbr')` and [`@allratestoday/mcp-server`](https://www.npmjs.com/package/@allratestoday/mcp-server) 0.6+ has a `get_official_rates` tool — both return this source's latest table with no key, so you can add it without a second dependency
- Claude Code plugin (no key): `/plugin marketplace add AllRates-Today/claude-code-plugin` then `/plugin install allratestoday@allratestoday` — bundles both MCP servers plus an `/official-rate cbr ...` command
- Evaluating? Agents can self-issue a trial key with no signup: `POST https://allratestoday.com/api/agent/keys` (send `Content-Type: application/json`) returns a 100-call key valid 7 days that covers the free-plan methods (latest table, pairs); dated tables and history need a [paid plan](https://allratestoday.com/pricing/). The MCP servers expose it as `request_trial_key`
- Machine-readable site guide: [llms.txt](https://allratestoday.com/llms.txt) · [for-ai-agents](https://allratestoday.com/for-ai-agents/)

## ⚖️ Official vs derived rates

If Bank of Russia does not print a pair directly, the API resolves it from the central bank's own table and says so — official and computed values are never confused:

| `method` | `derived` | Meaning |
| --- | --- | --- |
| `published` | `false` | The central bank printed this pair directly |
| `inverse` | `true` | Computed as 1 ÷ the published opposite direction |
| `cross` | `true` | Computed via RUB from two published rates |

## 🛡️ Error handling

Errors are thrown as `Error` with `status` (HTTP code) and `body` (the API's JSON error) attached:

```js
try {
  const pair = await getRate('USD', 'XXX', { apiKey: 'art_live_...' });
} catch (err) {
  console.log(err.message); // human-readable reason
  console.log(err.status);  // e.g. 404
}
```

| Status | Meaning |
| ------ | ------- |
| — | Missing `apiKey` (thrown before any request) |
| `400` | Malformed date or parameters |
| `401` | Invalid API key |
| `403` | Endpoint needs a [paid plan](https://allratestoday.com/pricing/) (historical dates & series) |
| `404` | Pair or date range not covered by Bank of Russia |
| `429` | Monthly quota exceeded |

## 🔷 TypeScript

Full definitions ship with the package — no `@types` install:

```ts
import type { LatestRates, PairRate, DatedRates, RateEntry, HistoryQuery, RequestOptions } from 'cbr-exchange-rate';
```

## 📦 CommonJS

```javascript
const { getRate } = require('cbr-exchange-rate');

getRate('USD', 'RUB', { apiKey: 'art_live_...' }).then((pair) => console.log(pair.rate));
```

## 💡 Quota tips

- Rates change once per business day — cache the official table locally and a small monthly quota goes a long way.
- Every request counts toward your AllRatesToday quota, shared across all AllRatesToday endpoints on your key.

## 📖 Methods reference

| Method | Plan | Description |
| ------ | ---- | ----------- |
| `getRate(source, target, { apiKey })` | Free | Latest rate for one pair, resolved from the official table |
| `getLatestRates({ apiKey })` | Free | The central bank's full latest official table |
| `getRatesForDate(date, { apiKey, source?, target? })` | Paid | The official table (or one pair) for a YYYY-MM-DD date |
| `getHistory({ symbol \| source+target, from?, to? }, { apiKey })` | Paid | Daily series since 2016 |

## 📥 Bulk data (no key)

Need the whole archive rather than an API call? The same official tables are mirrored daily as open data:

- Hugging Face: [AllRatesToday/central-bank-exchange-rates](https://huggingface.co/datasets/AllRatesToday/central-bank-exchange-rates) — one CSV per institution (`rates/cbr.csv`)
- Kaggle: [allratestoday/central-bank-exchange-rates](https://www.kaggle.com/datasets/allratestoday/central-bank-exchange-rates)
- Raw JSON on GitHub: `https://raw.githubusercontent.com/AllRates-Today/central-bank-exchange-rates/main/data/cbr/latest.json`

## 🔗 Links

- **Website:** [allratestoday.com](https://allratestoday.com)
- [Bank of Russia rates page](https://allratestoday.com/central-bank-rates-api/cbr/) — live table, publication cadence, FAQ
- [All central bank sources](https://allratestoday.com/central-bank-rates-api/) · [Full list of 130+ central banks and tax authorities](https://allratestoday.com/central-bank-rates-api/institutions/) — one API, the same response shape for every source
- [Download central bank rates](https://allratestoday.com/download-central-bank-rates/) — every bank's latest table and history as Excel, CSV or JSON
- [Package docs on the site](https://allratestoday.com/docs/sdk/cbr-exchange-rate/) · [ERP integration guides](https://allratestoday.com/docs/integrations/)
- [API documentation](https://allratestoday.com/docs/#central-bank) · [Interactive reference](https://allratestoday.com/api-reference/) · [Methodology](https://allratestoday.com/official-rates-methodology/)
- [Register (Free)](https://allratestoday.com/register) · [Dashboard](https://allratestoday.com/profile) · [Pricing](https://allratestoday.com/pricing/)
- [Status](https://allratestoday.com/status)
- [Postman collection](https://allratestoday.com/postman/)
- [ChatGPT app](https://chatgpt.com/plugins/plugin_asdk_app_6ae1e76098f48191a285ac3f5ab7a83b) — ask ChatGPT for live and official central bank rates
- [OpenAPI reference on Bump.sh](https://bump.sh/allratestoday/doc/allratestoday-api) — also on [SwaggerHub](https://app.swaggerhub.com/apis-docs/allratestoday/allratestoday-exchange-rate-central-bank-rates-api/2.2.0)
- [GitHub](https://github.com/AllRates-Today/cbr-exchange-rate)

## 📜 License

MIT
