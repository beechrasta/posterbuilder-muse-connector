# Setup prompt — paste into Meta Muse

Copy everything below the line into Muse:

---

Connect to the PosterBuilder API for me as a custom connector.

- API base: https://posterbuilder.vercel.app
- OpenAPI spec: https://posterbuilder.vercel.app/openapi.json
- Docs: https://posterbuilder.vercel.app/llms.txt

What it does: renders 1080x1080 social media posters and carousels. Three endpoints:

- `POST /api/render-poster` — single poster (headline, subtext, image URL, theme, template)
- `POST /api/render-deck` — multi-slide carousel deck
- `POST /api/generate-from-news` — takes raw news text, writes punchy copy, renders finished posters

No authentication needed — the API is public. Build the connector, then test it by rendering a poster that says "Hello from Muse", and confirm it is working.

---
