# Wykop MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wykop)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [news-media](../categories/news-media.md)

Read and analyze Wykop.pl — Poland's largest social news site and microblog: links, discussions, tag streams, search and user profiles, from your AI agent.

## Description
Connect your AI agent to **Wykop.pl**, Poland's largest social news aggregator and microblog (think Reddit + Twitter for the Polish internet), through its official API v3.

### What you can do

- **Link Discovery** — Browse the main page (`list_links` type_="homepage") or the upcoming queue ("upcoming"), ranked by newest, active, commented or most dug.
- **Discussion Reading** — Pull the comments of any link with `list_link_comments`, ranked by best/newest/oldest.
- **Microblog** — Read trending entries with `list_entries` (hot entries in a 1-12h window) and inspect single posts with `get_entry`.
- **Tag Streams** — Explore everything posted under a tag (e.g. #programowanie, #polityka) with `get_tag_stream`, filterable by year and month.
- **Search** — Search links, entries and users with `search` — supports @user and #tag prefixes.
- **Profiles** — Check any user's public profile, activity summary and followers with `get_profile`.

### How it works

1. Register an application at **dev.wykop.pl** to get your Application Key and Secret
2. Subscribe to this server and paste both credentials
3. Ask your agent for Polish news, discussions and community content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Market Researchers** — Track what the Polish internet is discussing right now.
- **Journalists & Analysts** — Monitor breaking stories, tag communities and public sentiment in Poland.
- **Community & Brand Managers** — Follow mentions, tag activity and discussion trends on the largest Polish social platform.


## Available Tools (8)
- **list_link_comments**: sort=best gives top-voted first, newest/oldest chronological. This is THE tool for reading link discussions. Paginate with page and limit (1-50).

Read the comment discussion of a Wykop link
- **get_entry**: Use it to inspect a specific entry found via list_entries or search. IDs are large integers.

Fetch a single microblog entry by ID with its content and vote stats
- **get_link**: Use it to inspect a specific link found via list_links or search. To read the discussion, feed the same id to list_link_comments. IDs are large integers.

Fetch a single Wykop link by ID with full details and vote stats
- **get_profile**: Use it to check who is behind a link or entry, or to gauge how active/influential a user is. The username is the handle without the @ (e.g. "wykop").

Fetch a Wykop user public profile: bio, location, links/entries activity summary and followers
- **get_tag_stream**: sort=all returns everything chronologically, best returns top-voted. Use for topic research: Polish communities organize heavily around tags like #programowanie, #polityka, #gamedev. Filter by year/month for historical research. Paginate with page and limit (1-50).

Browse all content under one Wykop tag (#hashtag) — entries and/or links
- **list_entries**: sort=hot gives the trending entries (combine last_update to window: 1,2,3,6 or 12 hours), newest gives latest, active gives most-recently-commented. Entries have text content, optional photo/embed, author and vote counts. Paginate with page and limit (1-50, default 20).

Browse the Wykop microblog ("wpisy") — short posts with votes, like a Polish Twitter/mastodon stream
- **list_links**: type_="homepage" returns links already promoted to the main page; type_="upcoming" returns the Wykopalisko queue (new links awaiting promotion). sort: newest, active, commented or digged. Each item has title, source URL, author, vote counts (up/down) and comment count — feed the id to get_link for details or list_link_comments for the discussion. Paginate with page and limit (1-50, default 20).

Browse Wykop.pl links (news posts) — main page or upcoming queue, with votes and comment counts
- **search**: type_ picks the result kind: links, entries, users or all. The query supports words plus prefixes: "@username" restricts to a user, "#tagname" to a tag. sort=score (relevance), popular, comments or newest. Results come back as link/entry/user objects — link and entry ids feed get_link/get_entry/list_link_comments. Search is Polish-content-first: try Polish phrasings for better recall. Paginate with page and limit (1-50, default 20).

Search Wykop links, entries and users by phrase — supports @user and #tag filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wykop** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's trending on Wykop.pl main page right now?"

**🤖 AI Agent:**
> Fetching the main page with `list_links`... Top story: a Polish tech article about new EU regulations with 340 up votes and 89 comments. Want me to read the discussion?

---

**👤 You:**
> "Search Wykop for recent posts about #programowanie (programming)."

**🤖 AI Agent:**
> Using `search` with query "#programowanie"... Found several recent entries: a thread about switching to Linux, a salary survey for Polish devs, and a link to a new Rust framework. Shall I pull the full comments of any of them?

---

**👤 You:**
> "What are the hottest microblog entries on Wykop in the last 6 hours?"

**🤖 AI Agent:**
> Fetching `list_entries` with sort=hot, last_update=6... The hottest is a post from a Polish startup founder with 210 up votes, followed by a viral political discussion.


## ❓ FAQ

**Q: Where do I get the Application Key and Secret?**
Register a new application at dev.wykop.pl (the official Wykop developer portal). Every Wykop API v3 request requires a JWT obtained with your application's key + secret — the server handles the login and token caching automatically.

**Q: Can the agent post, vote or comment for me?**
No — this server is read-only. It exposes public content discovery and analysis with application-level credentials; writing actions (adding links, posting entries, voting) require a user-authenticated token and are intentionally not included.

**Q: Is the content in Polish?**
Yes, Wykop content is overwhelmingly in Polish. The agent can still help you find and summarize discussions in English — use the search tool with Polish keywords or browse tag streams by topic for the best recall.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wykop](https://vinkius.com/ai-agent-connect/wykop)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wykop** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wykop` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wykop** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wykop": {
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
