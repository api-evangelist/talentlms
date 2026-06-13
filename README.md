# TalentLMS

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
