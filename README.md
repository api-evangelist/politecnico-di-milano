# Politecnico di Milano (politecnico-di-milano)

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

Politecnico di Milano is Italy's largest technical university — focused on engineering, architecture, and design — and is ranked #111 in the QS World University Rankings 2025. This repository catalogs its public, machine-readable developer/API footprint as an [APIs.json](https://apisjson.org) profile. That footprint is limited: there is no consolidated public developer portal. The most concrete public API is the OAI-PMH endpoint of the IRIS Re.Public@Polimi research repository, alongside an open data portal and a Shibboleth/SAML2 identity provider in the Italian IDEM (GARR) federation.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/politecnico-di-milano/refs/heads/main/apis.yml
- Run it with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=politecnico-di-milano-api-evangelist&utm_content=repo

## Type

- **Index** / **Consumer** / **3rd-Party**

## Tags

Education, Higher Education, University, Research, Open Data, Repository, OAI-PMH, Identity, Italy

## APIs

- **IRIS Re.Public@Polimi OAI-PMH** — Live OAI-PMH 2.0 metadata harvesting endpoint for the institutional research repository (CINECA "IRIS - POLIMI - prod"). Docs: https://re.public.polimi.it/ · Endpoint: https://re.public.polimi.it/oai/request?verb=Identify
- **Politecnico di Milano Open Data Portal** — Institutional open data portal; browse/download datasets, no documented programmatic API at review time. Docs: https://opendata.polimi.it/
- **Politecnico di Milano Shibboleth Identity Provider** — Shibboleth/SAML2 IdP providing federated SSO via the Italian IDEM (GARR) federation. Docs: https://www.polimi.it/onlineservices · Metadata: https://shibidp.polimi.it/idp/shibboleth

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/politecnico-di-milano-plans-pricing.yml](plans/politecnico-di-milano-plans-pricing.yml)
- Rate Limits: [rate-limits/politecnico-di-milano-rate-limits.yml](rate-limits/politecnico-di-milano-rate-limits.yml)
- FinOps: [finops/politecnico-di-milano-finops.yml](finops/politecnico-di-milano-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.polimi.it/en/
- LinkedIn: https://www.linkedin.com/school/polimi/
- Authentication (Shibboleth/SAML2 IdP): https://shibidp.polimi.it/idp/shibboleth
- Plans, Rate Limits, FinOps, and Review pointers (see above and [review.yml](review.yml))

## Notes

- All endpoints were probed live on 2026-06-03. The IRIS OAI-PMH endpoint returns a valid OAI-PMH 2.0 `Identify` response and a 200 on `ListMetadataFormats`.
- The open data portal (opendata.polimi.it) resolves but exposes no documented programmatic API — CKAN, Socrata, and `data.json` probes returned 404 — so it is cataloged as a data access point, not a confirmed machine API.
- A previously documented GPKB bioinformatics REST API (bioinformatics.deib.polimi.it/GPKB-REST/) now returns 404 and is excluded.
- No official Politecnico di Milano GitHub organization was confirmed; `github.com/POLIMI` is an unrelated account of student forks, and the real code lives in individual department/lab orgs. No GitHub common property is asserted.
- Community wrappers of the mobile-app/online-services backend exist on GitHub but are unofficial and archived; no endpoints from them were treated as official. No endpoints were fabricated.

## Maintainers

- Kin Lane — kin@apievangelist.com
