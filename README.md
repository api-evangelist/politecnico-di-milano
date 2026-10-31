# Politecnico di Milano

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

Politecnico di Milano is Italy's largest technical university — engineering, architecture and design — and a public research institution in Milan, ROR 01nffqt88. Like almost every university it is a federation of buyers rather than an API producer: there is no developer portal, no public API key, no status page and no changelog anywhere on polimi.it. What it does operate itself is real and was verified live on 2026-09-01. An open data portal at www.opendata.polimi.it publishes a DCAT-AP_IT catalogue in RDF Turtle describing 25 datasets, each with a CSV and a JSON distribution at a stable unauthenticated URL — all 25 returned 200 and 38,255 rows on probe, covering the course catalogue, enrolments, graduates, mobility, internships, grade distributions and research output under CC BY 4.0. Two separate OAI-PMH 2.0 endpoints are served from its own hosts: Re.Public@Polimi for research products and POLITESI for theses, the latter also harvestable in the DataCite kernel-4 metadata schema. It runs its own Shibboleth identity provider, shibidp.polimi.it, whose SAML 2.0 metadata is public and whose entityID is registered in the Italian IDEM GARR federation. Against that, the surfaces it does NOT own are recorded as such: the authenticated IRIS REST API on its repository host is CINECA's product contract, not the university's, and api.polimi.it is a live Kong gateway with no publicly routable endpoint behind it. This profile saves contracts only for the surfaces the institution itself operates.

**Areas:** Education · Higher Education · University · Technical University · Research · Open Data · Research Repository · Course Catalog · Identity Federation · OAI-PMH · Shibboleth · DCAT

## Politecnico di Milano on APIs.io

Everything profiled for Politecnico di Milano is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/politecnico-di-milano/](https://apis.io/providers/politecnico-di-milano/)** — or go straight to one of the APIs or properties below.

### APIs (7)

- [IDEM GARR Identity Federation membership](https://apis.io/apis/politecnico-di-milano/idem-garr-federation/) — Politecnico di Milano's membership of IDEM, the Italian academic identity federation run by GARR. The federation aggregate at md.idem.garr.it carries the…
- [ROR registration](https://apis.io/apis/politecnico-di-milano/ror-registration/) — The institution's entry in the Research Organization Registry, ROR ID 01nffqt88, carrying its canonical name in Italian, English and French and its own…
- [IRIS REST API (CINECA platform tenancy)](https://apis.io/apis/politecnico-di-milano/iris-rest/) — Politecnico di Milano's tenancy of CINECA's IRIS research information platform. The data is the university's; the contract is the vendor's, and it is not…
- [Politecnico di Milano Catalog API](https://apis.io/apis/politecnico-di-milano/politecnico-di-milano-catalog-api/) — The DCAT-AP_IT catalogue describing every published dataset.
- [Politecnico di Milano Distributions API](https://apis.io/apis/politecnico-di-milano/politecnico-di-milano-distributions-api/) — The CSV and JSON files each dataset is distributed as.
- [Politecnico di Milano Federation API](https://apis.io/apis/politecnico-di-milano/politecnico-di-milano-federation-api/) — SAML 2.0 metadata publication.
- [Politecnico di Milano Harvesting API](https://apis.io/apis/politecnico-di-milano/politecnico-di-milano-harvesting-api/) — The six OAI-PMH 2.0 verbs.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### JSON Schema (2)

The data models the API reads and writes.

- [Politecnico di Milano course catalog row](https://apis.io/schemas/politecnico-di-milano/politecnico-di-milano-course-catalog/)
- [Politecnico di Milano open data recordset](https://apis.io/schemas/politecnico-di-milano/politecnico-di-milano-opendata-recordset/)

#### JSON-LD (2)

Linked-data contexts for the provider's vocabulary.

- [Politecnico Di Milano Context](https://apis.io/jsonld/politecnico-di-milano/politecnico-di-milano-context/)
- [Politecnico Di Milano Opendata Catalog Context](https://apis.io/jsonld/politecnico-di-milano/politecnico-di-milano-opendata-catalog/)

#### Examples (1)

Example requests and responses.

- [Politecnico Di Milano Opendata Course Catalog](https://apis.io/examples/politecnico-di-milano/politecnico-di-milano-opendata-course-catalog/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Politecnico di Milano API Rules](https://apis.io/rules/politecnico-di-milano/politecnico-di-milano-spectral-ruleset/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Politecnico Di Milano Authentication](https://apis.io/security/politecnico-di-milano/politecnico-di-milano-authentication/)
- [Politecnico Di Milano Domain Security](https://apis.io/security/politecnico-di-milano/politecnico-di-milano-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Politecnico Di Milano Scopes](https://apis.io/scopes/politecnico-di-milano/politecnico-di-milano-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Politecnico Di Milano Plans Pricing](https://apis.io/plans/politecnico-di-milano/politecnico-di-milano-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Politecnico Di Milano Rate Limits](https://apis.io/rate-limits/politecnico-di-milano/politecnico-di-milano-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Politecnico Di Milano Finops](https://apis.io/finops/politecnico-di-milano/politecnico-di-milano-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.polimi.it/en/)
- [Support](https://www.polimi.it/en/the-politecnico/contacts)
- [Blog](https://www.polimi.it/en/the-politecnico/news)
- [Privacy policy](https://www.polimi.it/en/the-politecnico/communication/privacy)

## API Evangelist rating

**Kin Score 27.8** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 24.4 |
| Contract governance | 26.5 |
| Operational transparency | 5.3 |
| Developer ergonomics | 28.6 |
| Access clarity | 15.8 |

**Agent readiness 24.5** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | na |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | na |
| Error Semantics | — |
| OpenAPI Examples | verified |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | na |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 30.4** — Education & Research

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/politecnico-di-milano/](https://apis.io/providers/politecnico-di-milano/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Politecnico di Milano: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/politecnico-di-milano/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
