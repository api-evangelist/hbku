# Hamad Bin Khalifa University (hbku)

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
