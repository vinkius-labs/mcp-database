# TV Episode Sentinel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tv-episode-sentinel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [media-entertainment](../categories/media-entertainment.md)

Track new TV episodes and season progress across any show. Search the catalog, get everything aired since any date, next air dates and per-season progress — stateless, keyless, no account.

## Description
TV Episode Sentinel turns your agent into a "what's new on TV" watcher. It answers the questions people actually ask week after week: did anything new air of my shows, when is the next episode, and is the season over yet.

### What you can do

- **What's new since my last check** — pass any date and get every episode aired on or after it; the agent keeps your baseline, the server stays stateless
- **Watchlist in one call** — check up to 5 shows at once, staying under the source's rate limit instead of burning it with single calls
- **Next air dates** — the earliest scheduled episode, or a clear answer when nothing is scheduled
- **Season progress** — aired vs. total known episodes, last and next air dates, and whether the season is in progress or complete
- **Catalog search** — resolve any show name to its stable ID for the other tools

### How it works

1. Subscribe to this server (no credential, no account — the source API is public and anonymous)
2. Ask your agent "what new episodes of my shows aired since last week?" and keep the check date in your notes
3. Re-ask next week with the new date — only the delta comes back, never the whole history

The sentinel pattern is stateless by design: every "delta" tool takes a since date and returns only what changed after it. No databases, no stored watchlists, no per-user state — the agent's context is the memory.

### Who is this for?

- **TV watchers** — a weekly "what's new" digest for your favorite shows, no tracking the guide yourself
- **Agents & automations** — cheap, batched delta checks you can schedule without paying for full-history fetches
- **Researchers** — per-season progress and air-date audits across the catalog


## Available Tools (6)
- **next_aire**: Use this to answer "when does the next episode air?" If next is null, no future episode is scheduled (the show may have ended or dates may not be published yet).

The next scheduled episode of a show: airdate, season/episode and network
- **season_progress**: Use this to answer "how far along is season N?" or "is the season over?". Caveat: total_known counts episodes with published data, so a season that is still mid-run shows aired < total and upcoming episodes only when the network has published their air dates.

Progress of a season: how many of its known episodes have aired, last and next air dates
- **show_overview**: Use this to check whether a season is complete, when it ended, or what the show's schedule looks like. Pass a TVmaze ID when you have one to save a call.

Full overview of a TV show: status, network, schedule and every season with premiere/finale dates
- **find_shows**: Use this to resolve a show name into its ID before calling the other tools — every other tool accepts an ID or a name, but an ID avoids one extra lookup call. Cap the number of results with limit.

Search the TV catalog for shows by name or keyword and return their TVmaze IDs
- **new_episodes_since**: total_new counts everything matching; only up to max_results are listed. By default unaired (pre-scheduled) episodes are excluded — set include_scheduled to true to see them too. Keep your last-check date and pass it here as since to see only what is new since your last check. This is the tool to use whenever the question is "did anything new air of this show?".

New episodes of a show that aired on or after a given date — the core "what's new" query
- **watchlist_delta**: Shows that cannot be resolved are reported inline instead of failing the whole call. Use this for a standing watchlist: pass your last-check date as since, then update that date in your notes to the as_of value you receive. This batches network calls, which matters because the source is rate-limited to about 60 requests per minute.

Batch "what's new" check across up to 5 shows in one call


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TV Episode Sentinel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which new episodes of The Pitt aired since 2026-09-01?"

**🤖 AI Agent:**
> Uses new_episodes_since with since=2026-09-01 and returns the aired episodes newest-first.

---

**👤 You:**
> "Check my watchlist — what's new since last week for: The Pitt, Severance, The Bear?"

**🤖 AI Agent:**
> Uses watchlist_delta with the three names and since=last week's date; one batched call, per-show new-episode lists.

---

**👤 You:**
> "Is season 2 of Severance complete yet, and when does the next episode air?"

**🤖 AI Agent:**
> Uses season_progress for season 2 plus next_aire; reports aired/total known, last and next air dates.


## ❓ FAQ

**Q: Do I need an account or API key?**
No. Everything runs on the public anonymous endpoint (about 60 requests/minute). No signup, no key, no per-user state — the server is stateless and your agent keeps the baseline date in its own context.

**Q: How does "new since a date" work without the server remembering anything?**
It's the sentinel pattern: you (or your agent's notes) keep your last-check date, pass it as `since`, and the server fetches the show's episode list once and returns only episodes aired on or after that date. Re-run with the newer date next week and you get just the delta — never the full history again.

**Q: What happens when I hit the rate limit?**
The call returns an actionable error telling you to retry in about 60 seconds and to batch shows with `watchlist_delta` instead of separate calls — that one call checks up to 5 shows, which is usually comfortably under the limit.

**Q: Which shows and data does it cover?**
The full TVmaze catalog (scripted, reality, animation; US and international) with episode air dates, networks, season premiere/finale dates and status. If a show isn't in TVmaze, the search tool tells you so explicitly instead of failing silently.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tv-episode-sentinel](https://vinkius.com/en/ai-agent-connect/tv-episode-sentinel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TV Episode Sentinel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tv-episode-sentinel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TV Episode Sentinel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tv-episode-sentinel": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
