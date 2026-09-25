# ESPN Sports Sentinel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/espn-sports-sentinel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [monitoring](../categories/monitoring.md)

Know what's new in your league without re-reading the whole season: today's board (live, final, to play), completed games in the last days, upcoming games, one team's record and next game, league-wide injury news with a since-baseline, and a derived leaderboard. Keyless, stateless.

## Description
ESPN Sports Sentinel answers the question any sports fan has on a schedule: what changed in my league since the last time I looked? It reads the public ESPN site API — keyless, no account — and turns it into one stateless sentinel your agent can re-check on a schedule.

### What you can do

- **The daily pulse** — one league's whole board: what is live right now, what is final, what is still to play, with scores and records where known
- **What happened** — every decided game over the last N days (up to 7), sorted by date, with an empty-day note
- **What's coming** — the next N days of scheduled games (up to 14), including weeks when the league carries them
- **Follow one team** — current record, last N decided games with scores and venues, the result streak, and the next game
- **Injury news** — the league-wide injury list, or only entries reported since your last check (the since-baseline delta form)
- **A derived leaderboard** — win rates read from the recent boards, because the league's official standings table is not published as data

### How it works

1. Subscribe (no credential, no account — the ESPN site API is public)
2. Ask "what's going on in the NFL today?" — one call returns the live/final/to-play board
3. Keep the timestamp of the answer in context; on the next check pass it as since (injury_watch) or compare recent_games against your stored baseline — the agent reports only what changed

### Who is this for?

- **Fans and households** — a scheduled sports brief that only speaks when something is new
- **Agents & automations** — deltas over a league pulse: ticker, recent games, injuries since, derived standings, no full re-reads
- **Content & betting research** — the compact game lines, streaks and win-rate table as machine-readable inputs


## Available Tools (6)
- **injury_watch**: g. Injured Reserve), a short note and the reported date. Pass since (an ISO-8601 timestamp of your previous check) to see only what was reported after it — that is the delta form for scheduled watches. The list is capped at the first 40 rows and the result says when it was cut.

League-wide injury list, optionally only entries reported since a baseline timestamp
- **sports_ticker**: Pass a YYYYMMDD date to look at another day (including a past one — it becomes a score sheet); omit it for today. Zero games is a meaningful answer: off-season or a quiet day, said in the note. The agent should re-run this at its next check and diff against what it stored to report only what is new.

One-league pulse: what's live now, what's final, and what's still to play on that day's board
- **recent_games**: Days without decided games are listed in the note. Use it after the agent has a baseline of earlier results and wants only what finished since.

Completed games for one league over the last few days, sorted by date
- **team_follow**: ) or full name against the league team list, then reports its current W-L record, the last N decided games (default 5, max 15) with score, opponent and venue, its recent result streak (last up to 5 games, most recent first), and its next game. If the season has not produced a decided game yet, the record is reported as unknown with a note rather than invented.

Follow one team: current record, last N decided games, win/loss streak, and its next game
- **team_standings**: Only teams that actually played inside the window appear — that is the honest scope of a derived table, said in the note; expand the window to pull in more teams. Use it as the standing reference before comparing against what the agent stored earlier.

Derived leaderboard for one league: records and win rates of teams that played in the window
- **upcoming_games**: Early in the slate some games may still be named "TBD at TBD" until lineups lock in. Zero results is off-season or a quiet slate, said in the note — try a wider window before concluding.

Scheduled games for one league over the next few days, sorted by date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ESPN Sports Sentinel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's going on in the NFL today?"

**🤖 AI Agent:**
> Runs sports_ticker for nfl and reports the live, final, and still-to-play games with scores and records.

---

**👤 You:**
> "How have the Yankees been playing lately?"

**🤖 AI Agent:**
> Runs team_follow for mlb with team NYY and reports the current record, the last few decided games, the streak, and the next game.

---

**👤 You:**
> "Any new NBA injuries since 2026-09-20?"

**🤖 AI Agent:**
> Runs injury_watch for nba with since 2026-09-20T00:00:00Z and reports only the entries reported after that date.


## ❓ FAQ

**Q: Do I need credentials?**
No. The ESPN site API is public and anonymous — no key, no account. It does throttle anonymous bursts, so the tools are built to keep day windows small (a handful of scoreboard days, not season sweeps) and say so in the rate-limit note when it happens.

**Q: How does the "since" delta detection work?**
The server is stateless. Any tool that returns a timestamp is your baseline: keep it in the agent's context, and on the next check pass it as since. injury_watch then returns only the entries reported after that day — the agent reports the new news, not the whole list again. For games, compare a new recent_games answer against the games you stored.

**Q: Why is the leaderboard called "derived"?**
The league's official standings table is not published as queryable data in the 2026 API shape, so team_standings reads each team's W-L record from the scoreboard and schedule team objects over the last N days (default 14, max 30) and sorts by win rate. The honest scope: only teams that actually played inside the window appear — the result says so in its note. Widen the window to pull in more teams.

**Q: Which leagues are supported?**
Four US major leagues: MLB, NFL, NBA and NHL (pass mlb, nfl, nba or nhl, case-insensitive). Soccer was deliberately left out of this build — the same day-looping scoreboard pattern would work for it, so treat it as a follow-up rather than an oversight.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/espn-sports-sentinel](https://vinkius.com/en/ai-agent-connect/espn-sports-sentinel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ESPN Sports Sentinel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `espn-sports-sentinel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ESPN Sports Sentinel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "espn-sports-sentinel": {
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
