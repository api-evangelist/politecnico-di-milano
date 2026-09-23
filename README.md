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

Politecnico di Milano is Italy's largest technical university — engineering, architecture and design — and a public research institution in Milan (ROR [01nffqt88](https://ror.org/01nffqt88)). This repository catalogs its public, machine-readable footprint as an [APIs.json](https://apisjson.org) profile, under the API Evangelist **university pipeline**, whose first question is never "is there a spec" but **who operates the thing the spec describes**. Re-profiled 2026-09-01.

There is no developer portal, no public API key, no status page and no changelog on polimi.it. What the institution genuinely operates itself is smaller than a vendor's catalogue and entirely real: an open data portal publishing a DCAT-AP_IT catalogue in RDF Turtle over 25 live datasets, two separate OAI-PMH 2.0 endpoints, and its own Shibboleth identity provider registered in the Italian IDEM GARR federation.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/politecnico-di-milano/refs/heads/main/apis.yml
- Run it with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=politecnico-di-milano-api-evangelist&utm_content=repo

## Type

- **university** / **Technical University** / **Index** / **Provider** / **Public**

## Tags

Education, Higher Education, University, Technical University, Research, Open Data, Research Repository, Course Catalog, Identity Federation, OAI-PMH, Shibboleth, DCAT, Italy, Europe

## Surfaces, by operator

Every surface below carries an `x-operator` in `apis.yml`. `institution` means the university runs it and the contract is saved here. `tenant`, `federation` and `registry` are real institutional relationships whose contracts belong to somebody else and are deliberately **not** saved here.

### institution — contracts saved

- **Politecnico di Milano Open Data** — `https://www.opendata.polimi.it` — a DCAT-AP_IT catalogue in RDF Turtle at [/opendata_polimi.ttl](https://www.opendata.polimi.it/opendata_polimi.ttl) declaring 25 datasets, each with a CSV and a JSON distribution at a stable unauthenticated URL. All 25 JSON distributions returned 200 and 38,255 rows on 2026-09-01. CC BY 4.0. → [openapi](openapi/politecnico-di-milano-opendata-openapi.yml) · [schema](json-schema/politecnico-di-milano-opendata-recordset-schema.json) · [vocabulary](vocabulary/politecnico-di-milano-opendata-vocabulary.yml)
- **Re.Public@Polimi OAI-PMH** — `https://re.public.polimi.it/oai/request` — OAI-PMH 2.0 over the institutional research catalogue. `Identify` returns "IRIS - POLIMI - prod"; formats `oai_dc`, `didl`, `ore`. → [openapi](openapi/politecnico-di-milano-iris-oai-pmh-openapi.yml)
- **POLITESI OAI-PMH** — `https://www.politesi.polimi.it/oai/request` — a **second** OAI-PMH endpoint, over theses, additionally harvestable in the **DataCite kernel-4** metadata schema. Not recorded in any previous profile. → [openapi](openapi/politecnico-di-milano-politesi-oai-pmh-openapi.yml)
- **Shibboleth Identity Provider** — `https://shibidp.polimi.it/idp/shibboleth` — public SAML 2.0 metadata, scope `polimi.it`, signing and encryption keys valid to 2040. → [openapi](openapi/politecnico-di-milano-shibboleth-idp-openapi.yml)

### federation / registry / tenant — relationships recorded, contracts not saved

- **IDEM GARR federation** (`federation`) — the university's IdP entityID plus three of its service providers appear in the IDEM aggregate. A federation is shared by definition; the sharing is not misattribution.
- **ROR** (`registry`) — [ror.org/01nffqt88](https://ror.org/01nffqt88). A registry the institution is registered *in*.
- **IRIS REST API** (`tenant`) — `https://re.public.polimi.it/rest/api`, 401 Basic. Runs on the university's host, but the contract is CINECA's IRIS product. The tenancy is a real fact; the vendor's contract is not saved here.

## Domain standard conformance (Kin Score `education` regime)

Conformant: **oai-pmh** (two endpoints), **shibboleth**, **saml**. Partial: **datacite** (metadata schema served by POLITESI — but no DataCite registrant exists for this institution), **orcid** (iDs in Highwire citation meta tags on repository item pages, absent from the OAI-PMH output). Not found: crossref, scim, lti, oneroster, ed-fi, caliper, qti. Full evidence in [conformance/](conformance/politecnico-di-milano-conformance.yml).

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/politecnico-di-milano-plans-pricing.yml](plans/politecnico-di-milano-plans-pricing.yml)
- Rate Limits: [rate-limits/politecnico-di-milano-rate-limits.yml](rate-limits/politecnico-di-milano-rate-limits.yml)
- FinOps: [finops/politecnico-di-milano-finops.yml](finops/politecnico-di-milano-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-09-01

## Common Properties

- Website: https://www.polimi.it/en/
- Open data: https://www.opendata.polimi.it/
- Course catalog dataset: https://www.opendata.polimi.it/dataset/course_catalog/
- Research repositories: https://re.public.polimi.it/ · https://www.politesi.polimi.it/
- Identity federation: https://shibidp.polimi.it/idp/shibboleth
- AI policy: [Linee guida IA per il personale tecnico amministrativo](https://www.normativa.polimi.it/fileadmin/user_upload/regolamenti/privacy_e_sicurezza/LG_IA_PTA_v1.0def.pdf) · [normativa.polimi.it/privacy-e-sicurezza](https://www.normativa.polimi.it/privacy-e-sicurezza)
- Privacy: https://www.polimi.it/en/the-politecnico/communication/privacy
- LinkedIn: https://www.linkedin.com/school/polimi/

## Notes — what was probed, and what came back negative

- Everything above was probed live on **2026-09-01**. Every pointer emitted in `apis.yml` was re-fetched; all resolve (LinkedIn returns 999, its standard bot challenge, which grades as live).
- The open data portal was previously recorded as having **no documented programmatic API**. That was wrong, and instructively so: CKAN (`/api/3/action/package_list`), Socrata and `data.json` all 404 here, and the probe stopped there. The machine surface is a DCAT Turtle catalogue that the portal's own pages parse client-side with N3.js.
- `api.polimi.it` is a live **Kong 3.6.1** gateway on the institution's own domain, but every path probed (`/`, `/docs`, `/swagger`, `/openapi.json`, `/v1`, `/api`, `/health`, `/graphql`) returns `{"message":"no Route matched with those values"}`. No public API sits behind it, and none is claimed.
- `github.com/POLIMI` is **not** the university — an unrelated individual's organisation created in 2013 holding Coursera machine-learning exercises. No `GitHubOrganization` pointer is asserted.
- No **DataCite** registrant and no **Crossref** member matching this institution exist (`api.datacite.org/repositories?query=polimi` → 0; `api.crossref.org/members?query=politecnico` → unrelated matches). No DOI prefix is claimed.
- No `llms.txt`, no `.well-known/security.txt`, no status page, no changelog, no deprecation policy on any institution-operated surface.
- `trasparenza.polimi.it` publishes the D.Lgs 33/2013 data/metadata catalogue as HTML only — no machine-readable form.
- Searching in **Italian** mattered: both the AI governance documents and the open data catalogue are published only on Italian-language surfaces.
- Nothing here was fabricated. Every example in [examples/](examples/) is a live payload captured from the institution's own host, listed with its status code in [examples/politecnico-di-milano-examples.yml](examples/politecnico-di-milano-examples.yml).

## Maintainers

- Kin Lane — kin@apievangelist.com
