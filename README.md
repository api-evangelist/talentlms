# TalentLMS

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

TalentLMS is a cloud-based learning management system (LMS) with a REST API for managing users, courses, categories, branches, groups, and enrollments, as well as accessing completion and assessment report data.

## API

- **Developer Hub:** https://developers.talentlms.io/
- **API V2 Docs:** https://help.talentlms.com/hc/en-us/articles/24874457011356-TalentLMS-API-V2
- **Postman Collection:** https://documenter.getpostman.com/view/31867199/2sAY548Kou
- **Base URL (V2):** `https://{domain}.talentlms.com/api/v2`

## Authentication

TalentLMS uses API key authentication:

- **V1:** HTTP Basic Auth with the API key as the username and an empty password.
- **V2:** Header-based authentication using `X-API-Key: your_api_key` plus `X-API-Version: YYYY-MM-DD`.

API keys are generated in Account & Settings > Integrations > API within the TalentLMS admin portal.

## Key Resources

- Users
- Courses
- Categories
- Branches
- Groups
- Enrollments
- Reports (completion, assessment, test results, surveys)

## Rate Limits

- **V2:** 200 calls per 5 seconds; 2,000 calls per hour. Rate limit headers included in every response.
- **V1:** ~50 calls per hour (free tier); no rate limit headers.

## Pricing

Plans are based on monthly active users (users who log in during the billing period):

| Plan       | Price (yearly) | Users    |
|------------|---------------|----------|
| Free       | $0/month      | Up to 5  |
| Core       | $119/month    | Up to 40 |
| Grow       | $229/month    | Up to 70 |
| Pro        | $449/month    | Up to 100 (+$6/extra user) |
| Enterprise | Custom        | 1,000+   |

Annual billing provides a 20% discount.

## Links

- [Website](https://www.talentlms.com/)
- [Pricing](https://www.talentlms.com/pricing)
- [Blog](https://www.talentlms.com/blog/)
- [Support / Help Center](https://help.talentlms.com/hc/en-us)
- [Release Notes](https://help.talentlms.com/hc/en-us/sections/9593869767452-Product-News)

## APIs.json

This repository contains an [APIs.json 0.19](apis.yml) profile for TalentLMS maintained by [Kin Lane](mailto:kin@apievangelist.com) at [API Evangelist](https://apievangelist.com).
