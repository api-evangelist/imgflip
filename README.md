# Imgflip (imgflip)

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
