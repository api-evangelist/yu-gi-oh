# YGOPRODeck (yu-gi-oh)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

YGOPRODeck is a community-run Yu-Gi-Oh! TCG database and deck-sharing platform that exposes a free, public REST API (v7) for querying every Yu-Gi-Oh! card, archetype, card set, banlist status, format legality, market price, and card image. The API is the canonical open data source used by community deck builders, mobile apps, Discord bots, simulators, and analytics tools across the Yu-Gi-Oh! ecosystem.

**APIs.json:** [https://ygoprodeck.com/api-guide/](https://ygoprodeck.com/api-guide/)

## Tags

- Games
- Trading Card Games
- Yu Gi Oh
- Card Database
- Open Data
- Community API
- Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### YGOPRODeck Card Database API

The v7 REST API for the YGOPRODeck Yu-Gi-Oh! card database. Provides card search and filtering across every printed Yu-Gi-Oh! card, full card metadata (type, race, attribute, level, link, link markers, ATK/DEF, archetype, banlist, format legality), card sets and release info, archetypes, valid value enumerations, database version, and a random card endpoint. Free, no API key required, 20 requests per second per IP.

- **Human URL:** [https://ygoprodeck.com/api-guide/](https://ygoprodeck.com/api-guide/)
- **Base URL:** `https://db.ygoprodeck.com/api/v7`

#### Tags

- Games
- Trading Card Games
- Yu Gi Oh
- Card Database
- Card Search
- Archetypes
- Card Sets
- Pricing

#### Properties

- [Documentation](https://ygoprodeck.com/api-guide/)
- [Documentation](https://ygoprodeck.com/api-guide-supplemental/)
- [OpenAPI](openapi/yu-gi-oh-ygoprodeck-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/yu-gi-oh-ygoprodeck.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/yu-gi-oh-ygoprodeck.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Sign Up](https://ygoprodeck.com/account/)
- [SDK](https://github.com/Yeet195/pygo_API)
- [SDK](https://github.com/kaangiray26/pydeck)
- [SDK](https://github.com/RonaldTheodoro/ygoprodeck-api-client)
- [SDK](https://github.com/TheAnachronism/YGOPRODeck-Api-Wrapper)
- [SDK](https://github.com/MordechaiHadad/ygopro.NET)
- [SDK](https://github.com/whdzera/ygoprodeck)
- [Code Examples](https://github.com/fferegrino/yu-gi-oh)
- [Code Examples](https://github.com/usersina/YGOCards_Downloader)
- [Webhook](https://ygoprodeck.com/api-guide/)

## Common Properties

- [Website](https://ygoprodeck.com/)
- [Documentation](https://ygoprodeck.com/api-guide/)
- [Documentation](https://ygoprodeck.com/api-guide-supplemental/)
- [Pricing](https://ygoprodeck.com/premium/)
- [Public APIs Listing](https://github.com/public-apis/public-apis)
- [Third Party Open A P I](https://github.com/magicDGS-gaming/ygoprodeck-openapi)
- [Rate Limits](https://ygoprodeck.com/api-guide/)
- [Tools](https://github.com/Doarakko/draw-action)
- [Tools](https://github.com/Morphclue/ygo-bubble-tea)
- [Tools](https://github.com/BillyCool/YGOPRODeckArchive)
- [Tools](https://github.com/alisyedn/yugioh-mcp-server)
- [Tools](https://github.com/ludoplex/yugioh-mcp-server)
- [Vocabulary](vocabulary/yu-gi-oh-vocabulary.yml)
- [JSON-LD](json-ld/yu-gi-oh-ygoprodeck-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Spectral Rules](rules/yu-gi-oh-rules.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
