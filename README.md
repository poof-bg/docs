# Poof API docs

Source for [docs.poof.bg](https://docs.poof.bg), the developer documentation for the [Poof](https://poof.bg) background removal API. Built with [Mintlify](https://mintlify.com).

## Layout

- `mint.json` — site configuration and navigation
- `introduction.mdx`, `quickstart.mdx` — getting started
- `api-reference/` — endpoint pages (`POST /remove`, `GET /me`)
- `errors/` — one page per error code plus the `errors/list` reference
- `integrations/` — Python and TypeScript SDKs, n8n, Zapier, Make, MCP
- `openapi.json` — OpenAPI 3.1 spec that powers the API reference pages

## Local preview

```bash
npx mintlify dev
```

Then open `http://localhost:3000`.

## OpenAPI spec

`openapi.json` is mirrored to `poof/apps/gateway/openapi.json` in the main Poof repo. Keep the two files identical: change it here, then copy it over (or the other way round) in the same change.

## Deployment

Pushes to the default branch are deployed automatically by the Mintlify GitHub app.
