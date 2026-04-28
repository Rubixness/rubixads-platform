# RubixAds — AI Google Ads Intelligence

Live Google Ads management platform powered by Claude AI and MCP server.

## Deploy to Railway

1. Push this repo to GitHub
2. Create new Railway service → connect GitHub repo
3. Set environment variables:
   - `ANTHROPIC_API_KEY` — your Anthropic API key
4. Deploy — Railway auto-detects Node.js and runs `npm start`

## Architecture

- `server.js` — Express server, serves the dashboard and proxies Anthropic API calls
- `public/index.html` — The full RubixAds dashboard UI
- The dashboard chat connects to your MCP server on Railway for live Google Ads data
