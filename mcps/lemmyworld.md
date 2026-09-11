# Lemmy.World MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/lemmyworld)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Read and analyze lemmy.world — the largest Lemmy instance: posts, comment threads, communities, user profiles and the public moderation log, straight from your AI agent.

## Description
Connect any AI agent to **lemmy.world**, the largest Lemmy instance of the Fediverse, and explore its content through natural conversation.

### What you can do

- **Post Discovery** — Browse the instance frontpage or a specific community with `list_posts`, ranked by Hot, Top (day/week/month/all-time), New or Most Comments.
- **Thread Reading** — Pull the full comment tree of any post with `list_comments`, with configurable depth and Top/New ordering.
- **Community Research** — Search communities by keyword with `list_communities` and check subscriber counts and activity stats.
- **Search** — Keyword search across posts, comments, communities and users with `search`.
- **User Profiles** — Inspect a user's profile, recent posts and comments with `get_user`.
- **Instance Stats** — Get user/activity counts with `get_site_stats` and the transparency-friendly public moderation log with `get_modlog`.

### How it works

1. Subscribe to this server
2. Start querying — **no account or credentials needed**, all tools use the public API of lemmy.world
3. Ask your agent for posts, threads, communities or moderation history on lemmy.world from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Analysts** — Track discussions, sentiment and activity in open communities.
- **Community Managers** — Monitor what is being discussed and how communities are moderated.
- **Content Explorers** — Find the best threads and communities of the Fediverse without leaving your AI workflow.


## Available Tools (8)
- **list_posts**: Returns posts with title, URL, body excerpt, creator, community and engagement counts (score, comments). Without community_name you get the whole-instance feed; pass community_name (e.g. "technology") to see one community. Use sort to slice by relevance: Hot for what is trending now, TopDay/TopWeek/TopMonth for popular in a window, TopAll for the best ever, New for the latest. Paginate with page and limit (max 50) — do NOT expect all posts in one call. Combine with list_comments on a post id to read the discussion.

List posts on lemmy.world — the frontpage, a specific community, or top of a time window
- **get_post**: Use it to inspect a specific post found via list_posts or search. To read the discussion, feed the same id to list_comments. IDs are large integers (e.g. 51703042).

Fetch a single post by ID with full details and engagement counts
- **list_comments**: Pass post_id (from list_posts, get_post or search) to read that post's discussion — this is THE tool for reading replies. max_depth controls nesting (1 = top-level only, 3-6 shows the back-and-forth); sort=Top gives best-first, New gives latest. IMPORTANT: limit counts only TOP-LEVEL comments — nested replies up to max_depth are returned in addition, so a page can contain far more items than limit. Keep limit small (5-10) when max_depth > 1. Paginate with page for more top-level comments; deep threads may need several pages.

Read the comment thread of a post
- **list_communities**: Use q to filter by keyword (e.g. q="gaming") or omit it to list the biggest. sort=TopAll ranks by subscribers (stable); Hot ranks by current activity. Community names (for list_posts community_name) are lowercase, e.g. "technology", "asklemmy", "games". Paginate with page and limit (max 50).

Browse or search communities (subreddits) on lemmy.world, with subscriber counts
- **search**: type_ narrows the result kind: Posts, Comments, Communities, Users or Url (search by link URL); All returns every kind in one response. Results come back grouped per type with the matching views — post results include the post id you can feed to get_post/list_comments, community results include names usable in list_posts. sort=TopAll finds highest-scored matches; sort=New finds the freshest. Search is exact-keyword based (no fuzzy matching) — try multiple phrasings if results are thin. Paginate with page and limit (max 50).

Search posts, comments, communities and users on lemmy.world by keyword
- **get_user**: username is the local handle WITHOUT the @instance suffix (e.g. "ruud", not "ruud@lemmy.world"); for users federated from other instances, find their person_id via search (type_=Users) and pass person_id instead. Use it to check who is behind a post/comment or to see what someone has been posting.

Fetch a user profile by username with their recent posts and comments
- **get_site_stats**: Cheap and keyless — use it first to gauge instance size and activity, or to answer "how big is lemmy.world".

Instance-wide stats for lemmy.world: user counts, activity levels and admin list
- **get_modlog**: Use it for transparency checks: why a post disappeared, who got banned where, moderation patterns of a community (pass community_id from search results). Paginate with page and limit (max 50). Entries are newest-first.

Public moderation log: removed posts/comments, bans and community actions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lemmy.World** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the hottest posts on lemmy.world right now?"

**🤖 AI Agent:**
> Fetching the frontpage with `list_posts` sorted by Hot... Top right now: a thread on open-source alternatives with 340 comments, and a federated science post with a score of 1.2k.

---

**👤 You:**
> "Find gaming communities on lemmy.world with the most subscribers."

**🤖 AI Agent:**
> Using `list_communities` with q="gaming"... The largest are !games (78k subscribers), !patientgamers (92k) and !linux_gaming (45k). Want me to pull the top posts of any of them?

---

**👤 You:**
> "Why was the post "Fox News sharing billionaire propaganda" removed?"

**🤖 AI Agent:**
> Checking the public moderation log with `get_modlog`... Found it: removed by a moderator of !politics with reason "Not local politics. Just because a man is from Tucson doesn't mean it rises to local politics."


## ❓ FAQ

**Q: Do I need a Lemmy account or API key?**
No. All tools use the public API of lemmy.world and require no credentials — subscribe and start querying immediately.

**Q: Can the agent post, vote or comment for me?**
No — this server is read-only by design. It exposes discovery and analysis of public content; writing (posting, voting, commenting) requires an authenticated account and is intentionally not included.

**Q: Can I read content from other Lemmy instances or federated users?**
Yes, partially. lemmy.world federates with the whole Fediverse, so its feeds include federated posts, communities and users. Local usernames in get_user must be lemmy.world accounts; for federated users, find their person_id via search (type_=Users).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/lemmyworld](https://vinkius.com/en/ai-agent-connect/lemmyworld)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lemmy.World** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lemmyworld` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lemmy.World** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lemmyworld": {
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
