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

Hamad Bin Khalifa University (HBKU) is a research-intensive graduate university founded in 2010 within Qatar Foundation's Education City in Doha, Qatar, and ranked #183 in the QS World University Rankings 2025. This repository catalogs HBKU's public developer/API footprint as an APIs.json profile. HBKU does not operate a centralized public developer portal or documented institutional API; its most significant public, machine-readable surface is its scholarly research output deposited in Manara - Qatar Research Repository (Figshare-powered, hosted by Qatar National Library), accessible via Figshare's public REST API v2 and OAI-PMH endpoint.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=hbku-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Research, Open Access, Repository, Qatar, Middle East

## APIs

- **Figshare API v2 (Manara - HBKU Research)** — JSON REST API for HBKU research articles, datasets, and collections hosted in Manara. Docs: https://docs.figshare.com/ (base `https://api.figshare.com/v2`)
- **Figshare OAI-PMH (Manara - HBKU Research)** — OAI-PMH v2.0 metadata harvesting for HBKU works. Docs: https://help.figshare.com/article/how-to-use-the-oai-pmh (base `https://api.figshare.com/v2/oai`)

These are third-party platforms hosting HBKU content, not APIs operated by HBKU directly. No HBKU-operated public API was found.

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/hbku-plans-pricing.yml](plans/hbku-plans-pricing.yml)
- Rate Limits: [rate-limits/hbku-rate-limits.yml](rate-limits/hbku-rate-limits.yml)
- FinOps: [finops/hbku-finops.yml](finops/hbku-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.hbku.edu.qa/en/home
- GitHub: https://github.com/cri-lab-hbku
- LinkedIn: https://www.linkedin.com/school/hamad-bin-khalifa-university/
- Twitter/X: https://x.com/hbku
- Library: https://www.hbku.edu.qa/en/hbku-library
- Repository: https://manara.qnl.qa/hbku

## Notes

- No centralized HBKU developer portal or documented institutional API was found. Academic catalog (catalog.hbku.edu.qa), library OPAC/databases, and the Elmi research management portal resolve live but expose no public programmatic access.
- HBKU API surface cataloged here is hosted on third-party platforms (Figshare/Manara) with confirmed live public endpoints. No endpoints were fabricated.
- `cri-lab-hbku` is HBKU's Cybersecurity Research Lab GitHub org (public research repos), not a central university API org.
- Verification details and probed HTTP statuses are recorded in [review.yml](review.yml).

## Maintainers

- Kin Lane — kin@apievangelist.com
