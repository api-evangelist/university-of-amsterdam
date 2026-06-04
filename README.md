# University of Amsterdam (university-of-amsterdam)

The University of Amsterdam (Universiteit van Amsterdam, UvA) is a public research university in Amsterdam, Netherlands, ranked #43 in the QS World University Rankings 2025. This repository catalogs UvA's public developer/API footprint as an APIs.json provider profile. The confirmed public, machine-readable surface is centered on the University Library's open-data program — a Linked Open Data platform (Triply) plus OAI-PMH metadata endpoints — rather than a unified key-issuing developer portal.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-amsterdam-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Open Data, Linked Data, Library, Netherlands, Europe

## APIs

- **UvA Library Linked Open Data API (Triply)** — REST over the Library's LOD datasets (books, catalogue, images, letters, maps, audio, video, music, objects), backed by SPARQL/GraphQL/Elasticsearch.
  - Portal: https://lod.uba.uva.nl/
  - Base URL: https://api.lod.uba.uva.nl/datasets/UB-UVA/
  - Docs: https://docs.triply.cc/triply-api/
- **UvA Central Catalogue OAI-PMH** — metadata harvesting for the central library catalogue (Ex Libris Alma).
  - Base URL: https://uva.alma.exlibrisgroup.com/view/oai/31UKB_UAM1_INST/request
  - Docs: https://uba.uva.nl/en/support/open-data/data-sets-and-publication-channels/data-sets-and-publication-channels.html
- **UvA Archives Collection Descriptions OAI-PMH** — archival EAD collection descriptions.
  - Base URL: https://archives.uba.uva.nl/oai
- **UvA Research Data Repository OAI-PMH (Figshare)** — dataset metadata for the UvA research data portal.
  - Base URL: https://api.figshare.com/v2/oai

## Plans

- plans/university-of-amsterdam-plans-pricing.yml

## Rate Limits

- rate-limits/university-of-amsterdam-rate-limits.yml

## FinOps

- finops/university-of-amsterdam-finops.yml

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.uva.nl/en
- Developer Portal (library open data): https://uba.uva.nl/en/support/open-data/open-data.html
- GitHub: https://github.com/uva
- LinkedIn: https://www.linkedin.com/school/university-of-amsterdam/

## Notes

- All endpoints were probed on 2026-06-03. The Triply LOD API, LOD portal, Triply docs, archives OAI, Figshare OAI, official website, and GitHub org all returned HTTP 200.
- The Alma central-catalogue OAI endpoint is documented as public but returned HTTP 403 to a scripted request (bot/User-Agent gating); it is cataloged with that caveat.
- `api.uva.nl` is the Anton Pannekoek Institute for Astronomy website, not an API, and was deliberately excluded.
- LinkedIn returned HTTP 999 (standard LinkedIn anti-bot response), not a dead link.
- No unified key-issuing developer portal and no public SIS/course/timetable/identity API were found. No endpoints were fabricated.

## Maintainers

- Kin Lane — kin@apievangelist.com
