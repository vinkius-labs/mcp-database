# Letterboxd MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/letterboxd)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Letterboxd API v0 as an MCP: film search, full film details with rating histograms, member profiles and diaries — official HMAC-SHA256 signed API (access granted by request).

## Description
**Letterboxd** — the social film diary loved by cinephiles — and its official API v0 as a single MCP server.

### What you can do
- **Film search** — the full Letterboxd film database by name, with LIDs, years, runtimes and posters
- **Film details** — directors, cast, taglines and Letterboxd's famous weighted rating statistics (histogram from 0.5 to 5.0 stars)
- **Member profiles** — public profiles with films-watched, lists and fans counts
- **Member diaries** — recent logged films with dates, ratings and re-watch flags (member scope)

### Authentication (from the official API v0 docs)
1. Access to the Letterboxd API is **granted by request only** — email api@letterboxd.com with your project details (subject = app title)
2. Approved apps receive an **API key + API secret**
3. Every request is uniquely signed: add `apikey`, `nonce` (unique UUID) and `timestamp` (unix seconds) params, then append `signature` = lower-case hex HMAC-SHA256(apiSecret, METHOD + NUL + URL + NUL + JSON body)
4. Member tools (diary) use `POST /auth/token` with `grant_type=password` — the signature goes in the Authorization header for form-encoded POSTs

### Who is this for?
Film-data apps, statisticians, watchlist tools and AI agents bringing Letterboxd's social film data into conversations.


## Available Tools (6)
- **get_film_statistics**: 5-5.0 stars), weighted average rating, count of watches, lists and fans. The social analytics layer for films.

Get rating statistics for a film: weighted average, histogram, fans, watches, lists
- **get_film_details**: id = LID from search_films.

Get full film details by Letterboxd id: cast, crew, ratings statistics, runtimes
- **search_films**: Use film LIDs in get_film_details. Paged via perPage/page; also supports sort options (FilmName, FilmRating, ReleaseDateLatest...).

Search films in the Letterboxd database by name (and optionally release year)
- **search_members**: Use memberIds in member film/diary tools.

Search Letterboxd members by username (for profile and diary tools)
- **get_member_profile**: memberId from search_members.

Get a member profile: name, avatar, bio, stats (films watched, lists)
- **get_member_diary**: Requires member scope granted to your API key.

Get a member's diary: recent logged films with dates, ratings and re-watches


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Letterboxd** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search Letterboxd for 'In the Mood for Love' and give me the rating histogram"

**🤖 AI Agent:**
> 🎬 **In the Mood for Love (2000) — Wong Kar-wai**

Letterboxd weighted rating: **4.3/5**
Histogram: massive peak at 4★ and 4.5★, tiny tail below 2★
Fans: 250k+ · Watched: 1.2M+

One of the highest-rated films on the platform. Want the director's other films ranked by Letterboxd rating?

---

**👤 You:**
> "Find member 'boxd' and show their recent diary entries"

**🤖 AI Agent:**
> 🎬 **Member diary (Letterboxd)**

Recent log entries:
- 2026-09-05: Tenet (2020) — ★★★½, rewatch
- 2026-09-02: Perfect Days (2023) — ★★★★★

Ratings and re-watch flags pulled from the member's public diary. Want their watchlist too?

---

**👤 You:**
> "Compare Letterboxd ratings for Fight Club and Se7en"

**🤖 AI Agent:**
> 🎬 **Fight Club vs Se7en (Fincher double bill)**

- Fight Club: 4.3/5 weighted — stronger 4★/4.5★ concentration
- Se7en: 4.2/5 weighted — broader 3.5★-4★ spread

Fight Club edges it on Letterboxd. Want the full histograms or each film's most-rated year?


## ❓ FAQ

**Q: How do I get an API key?**
Letterboxd API access is granted by request only: email api@letterboxd.com describing your intended use (subject = your app/project title). Approved apps receive an API key + API secret. There is no self-service registration.

**Q: How does the request signing work?**
Every request adds apikey, nonce (unique UUID) and timestamp (unix seconds) params. The signature is the lower-case hex HMAC-SHA256 of the salted bytestring METHOD \0 fully-qualified URL \0 JSON body, using your API secret — appended as the final signature query parameter. Form-encoded POSTs (like /auth/token) put the signature in the Authorization header instead.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/letterboxd](https://vinkius.com/ai-agent-connect/letterboxd)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Letterboxd** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `letterboxd` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Letterboxd** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "letterboxd": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
