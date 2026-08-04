# Imgflip (imgflip)

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

Imgflip is a meme generator platform providing a REST API for captioning popular meme templates, searching over one million meme formats, auto-generating memes from text input, and creating original AI-powered meme images. Free endpoints cover getting popular templates and captioning images; premium endpoints unlock GIF captioning, meme search, automeme, and AI meme generation.

**APIs.yml:** [apis.yml](apis.yml)

## API

- **Imgflip Meme Generator API** — [Documentation](https://imgflip.com/api)
  - Base URL: `https://api.imgflip.com`
  - Auth: Username + password (Premium endpoints require API Premium subscription)
  - Format: REST / JSON

### Endpoints

| Endpoint | Method | Tier | Description |
|---|---|---|---|
| /get_memes | GET | Free | Retrieve array of popular meme templates |
| /caption_image | POST | Free | Add captions to image meme templates |
| /caption_gif | POST | Premium | Add captions to animated GIF templates |
| /search_memes | POST | Premium | Search 1M+ meme templates by query |
| /get_meme | POST | Premium | Retrieve a specific meme by ID |
| /automeme | POST | Premium | Auto-generate meme from text input |
| /ai_meme | POST | Premium | Create original memes via OpenAI GPT or Imgflip neural network |

## Plans & Pricing

| Plan | Price | Details |
|---|---|---|
| Free | $0/month | /get_memes and /caption_image, no hard rate limit, watermarked output |
| Premium | $9.99/month | All endpoints; monthly free allocations per endpoint type, then per-request overage fees |

## Rate Limits

- Free: No hard limit; throttling/blocking possible for abusive patterns
- Premium: Monthly free allocations per endpoint (50–200 requests); $0.005–$0.02 per request beyond allocation

## Tags

Memes, Images, GIFs, Entertainment, AI, Image Generation

## Links

- [API Documentation](https://imgflip.com/api)
- [Terms of Service](https://imgflip.com/terms)
- [Sign Up](https://imgflip.com/signup)

## Timestamps

- **Created:** 2026-06-13
- **Modified:** 2026-06-13

## Maintainers

- **Kin Lane** — kin@apievangelist.com
