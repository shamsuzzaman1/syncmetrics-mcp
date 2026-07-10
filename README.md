# SyncMetrics — MCP Server

**Ask Claude anything about your ads.** SyncMetrics is a remote [Model Context
Protocol](https://modelcontextprotocol.io) server that connects your marketing
accounts to Claude (and any MCP client) through one OAuth sign-in.

- **8 platforms:** Meta Ads, Google Ads, TikTok Ads & Organic, LinkedIn Ads,
  Google Analytics 4, Shopify, Facebook Pages, Google Sheets
- **106 tools** + 88 ready-made analysis recipes
- **Read-only by default** — the only writes are opt-in Google Ads campaign
  actions and Google Sheets exports, and every write is preview-first
  (new campaigns are always created paused)
- **Flat pricing, no AI credits** — 14-day free trial (no card), then $10–25/mo

## Connect

**Server URL:** `https://mcp.syncmetrics.io/mcp` — OAuth 2.1 + PKCE, no tokens to paste.

### In Claude
Settings → Connectors → **Add custom connector** → paste the URL above → sign in.

### In other MCP clients
Add a remote (streamable-http) server pointing at `https://mcp.syncmetrics.io/mcp`.

First connect your ad accounts at **[app.syncmetrics.io](https://app.syncmetrics.io)**,
then ask Claude things like *"How did my Meta ads do last week?"* or
*"Where am I wasting spend on Google Ads?"*.

## Links

- Website: https://syncmetrics.io
- Setup guide: https://syncmetrics.io/docs/connect
- Tool catalog (all 106): https://syncmetrics.io/docs/tools
- Recipes: https://syncmetrics.io/docs/recipes
- Privacy: https://syncmetrics.io/privacy · Support: https://syncmetrics.io/support

## About this repository

This repo is the **public registry record** for the SyncMetrics MCP server
(`server.json`) and connection docs. SyncMetrics is a hosted service — the server
itself runs at `mcp.syncmetrics.io`; the application source is proprietary. This
listing lets MCP registries and clients discover the connector.

_MCP is an open standard by Anthropic. SyncMetrics integrates with the official
Meta, Google, TikTok, LinkedIn, Shopify and Google APIs — no scraping._
