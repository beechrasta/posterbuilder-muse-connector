# PosterBuilder — Meta Muse Connector

The Meta Muse connector for **PosterBuilder**, the API that renders 1080x1080 social media posters and carousels. Tell Muse what you want a poster about; get back finished images.

- **Live API:** https://posterbuilder.vercel.app
- **OpenAPI spec:** https://posterbuilder.vercel.app/openapi.json
- **LLM docs:** https://posterbuilder.vercel.app/llms.txt

## What a Muse user can do

| Ask Muse | Route | Notes |
|---|---|---|
| "Make me a poster about [topic]" | `POST /api/render-poster` | Single 1080x1080 PNG: headline, subtext, image |
| "Make me a 5-slide carousel about [topic]" | `POST /api/render-deck` | Full multi-slide deck, every slide rendered |
| "Turn this news into posters" + pasted article | `POST /api/generate-from-news` | Writes the copy AND renders: headlines, subtext, images |

No auth. No API key. The API is public and free.

## Use it today — custom connector (no review, no wait)

Meta Muse can build a custom connector from any public API spec, with no directory approval needed:

1. Open Muse and paste the prompt from [SETUP-PROMPT.md](./SETUP-PROMPT.md).
2. Muse writes and tests the client in its VM and saves it.
3. Ask away: "make me a poster about..."

## Directory listing

Submitted for review in the Muse Connectors directory at [muse.ai/platform](https://muse.ai/platform). Once approved, it will be one tap in Settings → Connectors.

---

Built by [@beechrasta](https://github.com/beechrasta) · PosterBuilder app: https://posterbuilder.vercel.app
