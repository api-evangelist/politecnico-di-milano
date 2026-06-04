# Politecnico di Milano (politecnico-di-milano)

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
