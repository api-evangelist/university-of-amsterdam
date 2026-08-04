# University of Amsterdam (university-of-amsterdam)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
