# Hamad Bin Khalifa University (hbku)

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

Hamad Bin Khalifa University (HBKU) is a research-intensive graduate university founded in 2010 within Qatar Foundation's Education City in Doha, Qatar. This repository catalogs HBKU's public developer/API footprint as an APIs.json profile, with an explicit operator attribution on every surface.

HBKU's central administration publishes no developer portal, no open-data portal and no identity-federation entry. Its engineered API footprint comes from one research institute — the Qatar Computing Research Institute (QCRI), whose domain `qcri.org` redirects into `hbku.edu.qa` — which operates **Fanar**, Qatar's Arabic generative-AI platform, and **Farasa**, an Arabic NLP web API.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=hbku-api-evangelist&utm_content=repo

## Type

- Index / Provider / 1st-Party — `x-type: university`, `x-category: Private Research University`

## Tags

University, Higher Education, Education, Research, Qatar, Middle East, Artificial Intelligence, Large Language Models, Natural Language Processing, Arabic, Research Computing, Research Data, Course Catalog, Repository, Open Access

## APIs

Every entry carries an `x-operator`: who runs the thing the contract describes, which for a university is rarely the same answer as whose name is on the door.

**Institution-operated (HBKU's own engineering):**

- **Fanar API** (`x-operator: institution`) — Qatar's Arabic generative-AI platform, built by QCRI at HBKU with support from the Ministry of Communications and Information Technology. First-party OpenAPI 3.1.0 at https://api.fanar.qa/openapi.json — 11 paths, 12 operations, bearer auth, 14 documented error statuses behind one `Error` envelope, and a published per-model rate-limit table with `ratelimit-policy` headers. OpenAI-client compatible. Docs: https://api.fanar.qa/docs (base `https://api.fanar.qa`)
- **Farasa Web API** (`x-operator: institution`) — QCRI's Arabic NLP toolkit as a keyed web API. Six endpoints confirmed live by probe (segmentation, lemmatization, pos, ner, diacritize, spellcheck). The OpenAPI in this repo is **derived** from QCRI's own published code samples plus those probes, not published by the provider. Docs: https://farasa.qcri.org/ (base `https://farasa.qcri.org/webapi`)

**Tenant relationships (HBKU's data, someone else's contract) — recorded, not credited:**

- **Elmi Research Portal — OAI-PMH** (`x-operator: tenant`) — a working, unauthenticated OAI-PMH 2.0 endpoint over HBKU's Elsevier Pure instance at `https://elmi.hbku.edu.qa/ws/oai`, confirmed by `?verb=Identify` (adminEmail `elmi@hbku.edu.qa`), `ListMetadataFormats`, `ListSets` and `ListRecords`. This is the one education-regime domain standard HBKU meets. Pure's own REST API on the same host requires a key (401).
- **HBKU Academic Catalog — Course Search** (`x-operator: tenant`) — CourseLeaf JSON course-search at `https://catalog.hbku.edu.qa/course-search/api/`. Answers unauthenticated, but its backing term database is missing server-side, so it currently returns a fatal database error rather than course data.
- **Manara — Qatar Research Repository (HBKU portal)** (`x-operator: tenant`) — HBKU deposits on a Figshare platform operated by Qatar National Library. Behind an AWS WAF challenge (HTTP 202).

**Removed 2026-08-30:** eleven Figshare API definitions (`altmetric`, `articles`, `authors`, `collections`, `institutions`, `oauth`, `other`, `profiles`, `projects`, `symplectic`, plus the Figshare OAI-PMH entry) were recorded here as HBKU's own APIs. They were one Figshare contract — `info.title: Figshare API`, `contact: Figshare Support`, `servers: https://api.figshare.com/v2` — split eleven ways by tag, and the same document is shipped by a dozen other universities in this catalog. The specs and every artifact derived from them (collections, JSON Schema, JSON Structure, examples, rules, vocabulary, scopes, authentication, agentic-access, capability edges) have been removed. The relationship they misdescribed is preserved above as the Manara tenant entry.

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/hbku-plans-pricing.yml](plans/hbku-plans-pricing.yml) — both APIs are free, gated by request rather than payment
- Rate Limits: [rate-limits/hbku-rate-limits.yml](rate-limits/hbku-rate-limits.yml) — Fanar's real published per-model table
- FinOps: [finops/hbku-finops.yml](finops/hbku-finops.yml)

## Artifacts

- OpenAPI: [openapi/hbku-fanar-api-openapi.yml](openapi/hbku-fanar-api-openapi.yml) (`searched`), [openapi/hbku-farasa-api-openapi.yml](openapi/hbku-farasa-api-openapi.yml) (`derived`)
- Pristine source: [openapi/_original/hbku-fanar-api-openapi.json](openapi/_original/hbku-fanar-api-openapi.json)
- Errors: [errors/hbku-fanar-errors.yml](errors/hbku-fanar-errors.yml)
- Authentication: [authentication/hbku-authentication.yml](authentication/hbku-authentication.yml)
- JSON Schema: [json-schema/](json-schema/) · Examples: [examples/](examples/) · Rules: [rules/hbku-rules.yml](rules/hbku-rules.yml)
- Vocabulary: [vocabulary/hbku-vocabulary.yml](vocabulary/hbku-vocabulary.yml) · JSON-LD: [json-ld/hbku-context.jsonld](json-ld/hbku-context.jsonld)
- Conformance (education regime): [conformance/hbku-education-standards.yml](conformance/hbku-education-standards.yml) — 1 of 12 met (`oai-pmh`)
- Lifecycle: [lifecycle/hbku-lifecycle.yml](lifecycle/hbku-lifecycle.yml) · Domain security: [security/hbku-domain-security.yml](security/hbku-domain-security.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-30

## Common Properties

- Website: https://www.hbku.edu.qa/en/home
- Privacy Policy: https://www.hbku.edu.qa/en/privacy-policy
- Blog / News: https://www.hbku.edu.qa/en/news
- AI Tooling: https://fanar.qa/en
- Developer Portal: https://api.fanar.qa/docs
- Research Computing: https://www.hbku.edu.qa/en/qcri
- Research Repository: https://elmi.hbku.edu.qa/ (Elmi / Pure) · https://manara.qnl.qa/hbku (Manara / Figshare)
- Course Catalog: https://catalog.hbku.edu.qa/
- Library: https://www.hbku.edu.qa/en/hbku-library
- GitHub Organization: https://github.com/qcri
- Models: https://huggingface.co/QCRI
- LinkedIn: https://www.linkedin.com/school/hamad-bin-khalifa-university/
- X: https://x.com/hbku

## Notes

- Every pointer emitted here was fetched on 2026-08-30 and graded on its status code, not on its presence. Soft-404s were caught by body comparison: `fanar.qa/en/terms` and `fanar.qa/en/release-notes` return HTTP 200 with the homepage shell, while `fanar.qa/en/terms-of-services` and `fanar.qa/en/2-0-release-notes` are the real pages.
- Probed negatives: `data.hbku.edu.qa`, `sis.hbku.edu.qa`, `banner.hbku.edu.qa` and `idp.hbku.edu.qa` do not resolve; `sso.hbku.edu.qa` serves a certificate that does not match the hostname; `www.hbku.edu.qa/.well-known/security.txt` and `/llms.txt` return 404; `api.hbku.edu.qa` resolves but a BIG-IP WAF rejects every request. HBKU is in no eduGAIN federation — none of eduGAIN's 92 federations is Qatari and no `hbku.edu.qa` entity is registered.
- No endpoints were fabricated. Where a response shape could not be observed without a credential — Farasa's 200 body, Fanar's authenticated responses — no schema is asserted and the artifact says so.
- Verification details and probed HTTP statuses are recorded in [review.yml](review.yml) and in `x-coverage` in [apis.yml](apis.yml).

## Maintainers

- Kin Lane — kin@apievangelist.com
