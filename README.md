# YGOPRODeck (yu-gi-oh)

YGOPRODeck is a community-run Yu-Gi-Oh! TCG database and deck-sharing platform that exposes a free, public REST API (v7) for querying every Yu-Gi-Oh! card, archetype, card set, banlist status, format legality, market price, and card image. The API is the canonical open data source used by community deck builders, mobile apps, Discord bots, simulators, and analytics tools across the Yu-Gi-Oh! ecosystem.

**URL:** [Visit APIs.json URL](https://ygoprodeck.com/api-guide/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Type

- **x-type:** opensource (community)
- **x-tier:** 3 (bulk-registered from public-apis, enriched 2026-05-30)
- **source:** [public-apis/public-apis](https://github.com/public-apis/public-apis) — category: Games & Comics

## Tags

- Games, Trading Card Games, Yu Gi Oh, Card Database, Open Data, Community API, Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### YGOPRODeck Card Database API

The v7 REST API for the YGOPRODeck Yu-Gi-Oh! card database. Provides card search and filtering across every printed Yu-Gi-Oh! card, full card metadata (type, race, attribute, level, link, link markers, ATK/DEF, archetype, banlist, format legality), card sets and release info, archetypes, valid value enumerations, database version, and a random card endpoint. Free, no API key required, 20 requests per second per IP.

**Human URL:** [https://ygoprodeck.com/api-guide/](https://ygoprodeck.com/api-guide/)

**Base URL:** `https://db.ygoprodeck.com/api/v7`

#### Tags

- Games, Trading Card Games, Yu Gi Oh, Card Database, Card Search, Archetypes, Card Sets, Pricing

#### Properties

- [Documentation](https://ygoprodeck.com/api-guide/)
- [Documentation — Supplemental API Guide](https://ygoprodeck.com/api-guide-supplemental/)
- [OpenAPI](openapi/yu-gi-oh-ygoprodeck-openapi.yml)
- [NaftikoCapability — Cards](capabilities/ygoprodeck-cards.yaml)
- [NaftikoCapability — Card Sets](capabilities/ygoprodeck-card-sets.yaml)
- [NaftikoCapability — Archetypes](capabilities/ygoprodeck-archetypes.yaml)
- [NaftikoCapability — Reference Data](capabilities/ygoprodeck-reference-data.yaml)
- [NaftikoCapability — Database](capabilities/ygoprodeck-database.yaml)
- [SignUp](https://ygoprodeck.com/account/)
- [SDK — Python SDK (pygo_API)](https://github.com/Yeet195/pygo_API)
- [SDK — Python SDK (pydeck)](https://github.com/kaangiray26/pydeck)
- [SDK — Python Client (ygoprodeck-api-client)](https://github.com/RonaldTheodoro/ygoprodeck-api-client)
- [SDK — .NET / C# SDK (YGOPRODeck-Api-Wrapper)](https://github.com/TheAnachronism/YGOPRODeck-Api-Wrapper)
- [SDK — .NET Wrapper (ygopro.NET)](https://github.com/MordechaiHadad/ygopro.NET)
- [SDK — JavaScript / TypeScript Wrapper](https://github.com/whdzera/ygoprodeck)
- [CodeExamples — Card Dataset (Weekly Snapshot)](https://github.com/fferegrino/yu-gi-oh)
- [CodeExamples — Image Downloader (Python)](https://github.com/usersina/YGOCards_Downloader)
- [Webhook — Image Hotlinking Policy (do not hotlink)](https://ygoprodeck.com/api-guide/)

## Common Properties

- [Website](https://ygoprodeck.com/)
- [Documentation](https://ygoprodeck.com/api-guide/)
- [Documentation — Supplemental API Guide](https://ygoprodeck.com/api-guide-supplemental/)
- [Pricing — YGOPRODeck Premium (supports the free API)](https://ygoprodeck.com/premium/)
- [PublicAPIsListing](https://github.com/public-apis/public-apis)
- [ThirdPartyOpenAPI — magicDGS-gaming/ygoprodeck-openapi](https://github.com/magicDGS-gaming/ygoprodeck-openapi)
- [RateLimits — 20 Requests per Second per IP (1 hour ban on violation)](https://ygoprodeck.com/api-guide/)
- [Tools — Draw Yu-Gi-Oh! Card GitHub Action](https://github.com/Doarakko/draw-action)
- [Tools — YGO Bubble Tea CLI](https://github.com/Morphclue/ygo-bubble-tea)
- [Tools — YGOPRODeckArchive (.NET archiver)](https://github.com/BillyCool/YGOPRODeckArchive)
- [Tools — MCP Server (alisyedn/yugioh-mcp-server)](https://github.com/alisyedn/yugioh-mcp-server)
- [Tools — MCP Server (ludoplex/yugioh-mcp-server — PSCT + ruling engine)](https://github.com/ludoplex/yugioh-mcp-server)
- [Vocabulary](vocabulary/yu-gi-oh-vocabulary.yml)
- [JSONLD](json-ld/yu-gi-oh-ygoprodeck-context.jsonld)
- [SpectralRules](rules/yu-gi-oh-rules.yml)

## Features

| Name | Description |
|------|-------------|
| Card Search | Query the full Yu-Gi-Oh! card database with rich filters — exact name, fuzzy name, passcode ID, type, race, attribute, level/rank, link rating, link markers, ATK/DEF (with lt/lte/gt/gte comparison operators), pendulum scale, archetype, card set, format legality, banlist status, and effect-presence flag. |
| Multilingual Card Data | Retrieve card text in English (default), French, German, Italian, and Portuguese using the `language` parameter on the cardinfo endpoint. |
| Format and Banlist Filtering | Filter the catalog by tournament format (TCG, OCG, Goat, OCG Goat, Speed Duel, Master Duel, Rush Duel, Duel Links, GenesYS) and banlist status to power deck builders, legality checkers, and tournament tools. |
| Card Set and Print Run Catalog | Enumerate every Yu-Gi-Oh! card set (1,000+) with TCG release dates, card counts, set images, and per-print pricing and rarity data via cardsets.php and cardsetsinfo.php. |
| Archetype Catalog | List every recognised Yu-Gi-Oh! archetype (600+) to power archetype-based filtering, deck categorisation, and search-as-you-type experiences. |
| Market Price Aggregation | Each card response includes prices from Cardmarket, TCGplayer, eBay, Amazon, and CoolStuffInc to power price tracking and arbitrage tools. |
| Card Image CDN | Full-resolution, small, and cropped card images are served from images.ygoprodeck.com. Direct hotlinking is prohibited; consumers must download and self-host images. |
| Database Version Tracking | The checkDBVer.php endpoint exposes the current database version and last update timestamp so that cached clients can invalidate efficiently. |
| Random Card Endpoint | The randomcard.php endpoint returns a single random card and is uncached, suitable for "card of the day" widgets, Discord bots, and discovery features. |
| Open and Free Access | No API key, no authentication, no quota beyond the documented 20 requests per second per IP. Funded by YGOPRODeck Premium subscriptions, ads, and donations rather than API metering. |

## Use Cases

| Name | Description |
|------|-------------|
| Deck Builder | Web and mobile deck builders use cardinfo.php with archetype, format, and banlist filters to surface only the cards a player can legally include in a given tournament format. |
| Yu-Gi-Oh! Discord Bots | Discord bots like the official YGOPRODeck bot use cardinfo.php and randomcard.php to look up cards, post random cards, and resolve archetype questions inside chat servers. |
| Price Tracker | Apps that surface card prices use the per-card prices array to monitor Cardmarket/TCGplayer values, build watchlists, and detect arbitrage opportunities across marketplaces. |
| Tournament Legality Checker | Tournament platforms (Master Duel, Duel Links, TCG, OCG) use the banlist and format filters to confirm deck legality before accepting a registration. |
| Card Image Pipeline | Game simulators and printing tools download the full card image library once and rebuild their local card art catalog on each database version bump. |
| Card Recognition Training Data | Computer vision pipelines for physical card recognition pull the entire image set as labelled training data, keyed by card id. |
| Meta and Format Analytics | Meta analytics sites pull archetype and format data to build win-rate dashboards, archetype popularity charts, and ban-list impact studies. |

## Integrations

| Name | Description |
|------|-------------|
| Cardmarket | Per-card pricing in cardinfo responses sources Cardmarket marketplace prices. |
| TCGplayer | Per-card pricing in cardinfo responses sources TCGplayer marketplace prices. |
| eBay | Per-card pricing in cardinfo responses sources eBay listings. |
| Amazon | Per-card pricing in cardinfo responses sources Amazon listings. |
| CoolStuffInc | Per-card pricing in cardinfo responses sources CoolStuffInc marketplace prices. |
| Konami / 4K Media | All card text and imagery is copyright Konami Digital Entertainment / 4K Media; YGOPRODeck surfaces and redistributes it under fair-use community-database conventions. |

## Solutions

| Name | Description |
|------|-------------|
| Community Yu-Gi-Oh! Database | A fully open, community-maintained replacement for proprietary Yu-Gi-Oh! card databases that lets developers build any tool — deck builder, simulator, scanner, bot — on top of the complete TCG corpus without contractual gates. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [YGOPRODeck Yu-Gi-Oh! Card Database API v7](openapi/yu-gi-oh-ygoprodeck-openapi.yml) — 7 operations, 16 component schemas, full enum and parameter coverage

### JSON Schema

15 standalone JSON Schema files (draft 2020-12) in [`json-schema/`](json-schema/), one per OpenAPI component schema:

- Archetype, Card, CardClassValues, CardImage, CardMiscInfo, CardPrice, CardPrintingEntry, CardSearchResponse, CardSet, CardSetPrint, CardTypeEntry, CardValues, DatabaseVersion, MonsterValues, SearchMeta

### JSON Structure

15 JSON Structure (json-structure.org) files in [`json-structure/`](json-structure/), one per JSON Schema — strict-typed conversion using `int32`, `datetime`, `date`, and `uri` types.

### JSON-LD

- [YGOPRODeck JSON-LD Context](json-ld/yu-gi-oh-ygoprodeck-context.jsonld) — 73 property mappings + 15 type declarations linking YGOPRODeck card terms to `schema.org`, `dcterms`, and a `ygo:` namespace.

### Examples

15 example JSON payloads in [`examples/`](examples/), one per JSON Schema, populated with realistic Yu-Gi-Oh! card data (Dark Magician, Blue-Eyes White Dragon, Legend of Blue Eyes set, etc.).

## Capabilities

Naftiko capabilities organised one-file-per-OpenAPI-tag. Each file is self-contained and ships both a REST adapter (port 8080, `/v1/...` paths) and an MCP adapter (port 9090, verb-noun tool names).

| Capability | Tag | Operations | File |
|------------|-----|-----------:|------|
| YGOPRODeck — Cards | Cards | 2 | [capabilities/ygoprodeck-cards.yaml](capabilities/ygoprodeck-cards.yaml) |
| YGOPRODeck — Card Sets | Card Sets | 2 | [capabilities/ygoprodeck-card-sets.yaml](capabilities/ygoprodeck-card-sets.yaml) |
| YGOPRODeck — Archetypes | Archetypes | 1 | [capabilities/ygoprodeck-archetypes.yaml](capabilities/ygoprodeck-archetypes.yaml) |
| YGOPRODeck — Reference Data | Reference Data | 1 | [capabilities/ygoprodeck-reference-data.yaml](capabilities/ygoprodeck-reference-data.yaml) |
| YGOPRODeck — Database | Database | 1 | [capabilities/ygoprodeck-database.yaml](capabilities/ygoprodeck-database.yaml) |

## Vocabulary

- [YGOPRODeck Vocabulary](vocabulary/yu-gi-oh-vocabulary.yml) — Unified taxonomy mapping 5 resources, 3 actions, 5 workflows, and 4 personas across operational (OpenAPI) and capability (Naftiko) dimensions.

## Rules

- [YGOPRODeck Spectral Rules](rules/yu-gi-oh-rules.yml) — 36 rules across 10 categories (info / metadata, OpenAPI version, servers, paths, operations, tags, parameters, responses, schemas, security, HTTP methods, general quality) enforcing the YGOPRODeck v7 conventions (snake_case parameters, snake_case properties, camelCase operationIds, `YGOPRODeck` summary prefix, `.php` flat paths, GET-only methods, no security schemes).

## Pipeline Notes

This repository was profiled with the API Evangelist `opensource` pipeline (18 steps). Steps 14-16 (plans / rate-limits / finops) were skipped because YGOPRODeck is a free community service without a metered commercial API tier. Step 3b (discover-crds) was skipped because YGOPRODeck has no Kubernetes-native APIs.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
