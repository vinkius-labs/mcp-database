# Dev.to Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/devto-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Publish, manage, and deeply analyze Dev.to content with 22 tools — including proprietary intelligence modules for timing optimization, audience mapping, and content strategy.

## Description
**Goal:** Transform Dev.to from a simple publishing platform into a data-driven content intelligence engine for autonomous agents.

**Problem:** Most Dev.to integrations are thin API wrappers — search articles, publish, done. They offer no strategic insight into *when* to publish, *what* title format works best, or *which* adjacent communities share your audience. Content creators publish blindly, missing peak engagement windows and overlooking high-opportunity tags.

**Mechanism:** This server provides 22 tools organized in three tiers:

*Tier 1 — Content Management (14 tools):*
`search_articles`, `get_latest_articles`, `get_article`, `get_article_by_slug`, `get_comments`, `get_comment_by_id`, `get_tags`, `get_followed_tags`, `get_user`, `get_my_articles`, `get_my_drafts`, `get_reading_list`, `get_followers`, `get_podcast_episodes`.

*Tier 2 — Community Interaction (3 tools):*
`publish_article` creates articles with full markdown, canonical URL, and tag support. `update_article` modifies existing posts. `toggle_reaction` engages with content via likes, unicorns, or bookmarks.

*Tier 3 — Proprietary Intelligence (5 tools):*
- `analyze_engagement`: Deep-dives into a single article — comment sentiment, unique commenters, engagement score, estimated reach.
- `discover_top_authors`: Ranks the most influential authors for any tag by aggregating multi-article engagement data.
- `content_gap_analysis`: Compares up to 8 tags to find high-engagement topics with low competition.
- `publish_timing_analysis`: Cross-references ~120 article timestamps with engagement metrics to find the optimal day and reading-time sweet spot.
- `audience_crossover`: Multi-hop intelligence — traces commenters across tags to map hidden audience overlaps.
- `content_blueprint`: Reverse-engineers the structural patterns (title format, reading time, tag combos) of top-performing articles.

**Advantage:** The intelligence tier requires 20-40 orchestrated API calls per analysis — these are composite computations that cannot be replicated with a single endpoint. The engagement-weighted algorithms, opportunity scoring, and audience tracing provide genuinely proprietary strategic output that turns raw platform data into actionable publishing decisions.


## Available Tools (23)
- **get_my_drafts**: Use to review pending content, resume unfinished articles, or decide what to publish next.

Get your unpublished draft articles on Dev.to (requires API key)
- **analyze_engagement**: Use to evaluate content performance, benchmark against competitors, and identify what drives engagement. The engagement score weights comments 3x higher than reactions (comments = deeper engagement) and unique commenters 5x (community breadth).

Deep engagement analysis of a Dev.to article — reactions, comments, unique commenters, estimated reach, and engagement score
- **content_gap_analysis**: Computes an opportunity score: tags with high average engagement but low article volume represent content gaps. Use for strategic content planning — publish in high-opportunity tags to maximize reach with less competition.

Analyze content gaps across multiple tags — find high-engagement topics with low competition
- **get_followers**: Use for audience analysis, engagement planning, and community growth tracking.

Get your Dev.to followers (requires API key)
- **discover_top_authors**: Returns up to 15 top authors with their article count, engagement metrics, and best-performing article. Use for competitive intelligence — understand who dominates specific topics and what content style performs best.

Discover the most influential authors for a specific tag on Dev.to
- **toggle_reaction**: Categories: "like" (heart), "unicorn" (special appreciation), "readinglist" (bookmark/save). If the reaction already exists, it will be removed. Use to engage with community content — liking articles boosts their visibility.

Toggle a reaction (like, unicorn, or bookmark) on an article or comment (requires API key)
- **update_article**: You can modify the title, body, tags, description, canonical URL, or series. Use to fix typos, update content, add canonical URLs, or unpublish articles.

Update an existing Dev.to article (requires API key)
- **audience_crossover**: Reveals hidden audience connections. If your #mcp audience also writes #ai-agents and #devtools, cross-posting to those tags reaches the same people. This operation makes 20-40 API calls — genuine competitive intelligence that requires orchestration.

Map audience overlap — trace commenters in a tag to discover which OTHER tags they write about
- **content_blueprint**: Produces a data-driven "content recipe" that tells you exactly what to write and how to structure it. Unlike generic advice, this is derived from real engagement data.

Extract the structural recipe of top-performing articles in a tag — title patterns, optimal reading time, best tag combos
- **get_article_by_slug**: Use when you have the URL path (e.g. "ben/my-article-slug") instead of the numeric ID.

Get the full content of a Dev.to article by username and slug
- **get_article**: Use to analyze article structure, read full content, or prepare updates.

Get the full content of a single Dev.to article by ID
- **get_comment_by_id**: Use to follow up on specific discussions, analyze individual comment threads, or track responses to your content.

Get a single comment by its ID, including child replies
- **get_comments**: Use for sentiment analysis, community feedback review, and understanding reader engagement with specific content.

Get all comments on a Dev.to article
- **get_followed_tags**: Use to understand your content interests, align publishing strategy with followed topics, and discover your engagement profile.

Get tags you are following on Dev.to (requires API key)
- **get_latest_articles**: to community. Use for content discovery, trend monitoring, and understanding what topics are being actively discussed.

Get the most recently published articles on Dev.to
- **get_my_articles**: Use to audit your content performance, find articles to update, or review your publication history.

Get your own published articles on Dev.to (requires API key)
- **get_podcast_episodes**: Optionally filter by podcast username. Use for content discovery beyond articles — podcasts represent high-engagement multimedia content in the dev community.

Browse podcast episodes published on Dev.to
- **get_reading_list**: Use to review saved content, extract ideas from curated reading, or manage your knowledge pipeline.

Get your Dev.to reading list (bookmarked articles, requires API key)
- **get_tags**: Use for content strategy — understand which topics have the most engagement and readership on the platform.

Get popular tags on Dev.to
- **get_user**: Use to research authors, verify identities, or understand the audience behind specific content.

Get a Dev.to user profile by username
- **publish_article**: Provide the title, full Markdown body, and up to 4 tags. Optionally set a canonical URL (for SEO), series name (for multi-part content), and description (for meta). The article will be published immediately unless you set published to false (creates a draft).

Publish a new article on Dev.to (requires API key)
- **publish_timing_analysis**: Outputs: best/worst day of the week, day-by-day breakdown, optimal reading time range. This is a multi-call statistical analysis that cannot be replicated with a single API request. Use to time your content for maximum visibility.

Analyze optimal publishing times for a tag — best/worst days, reading time sweet spot, statistical breakdown
- **search_articles**: to community for articles. Filter by tag (e.g. "javascript", "ai", "webdev"), by author username, or by top articles in the last N days. Results include reactions, comments, and reading time for quick evaluation.

Search Dev.to articles by tag, username, or popularity. Returns published articles with engagement metrics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dev.to Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the best time to publish an article about AI agents on Dev.to."

**🤖 AI Agent:**
> Running `publish_timing_analysis` for #ai-agents: analyzed 97 articles. Best day: Tuesday (42 avg reactions). Worst day: Saturday (8 avg reactions). Reading time sweet spot: 5-8 minutes (51 avg reactions in range). Publish on Tuesday morning for maximum visibility.

---

**👤 You:**
> "What topics does the #mcp community also care about? I want to expand my reach."

**🤖 AI Agent:**
> Running `audience_crossover` for #mcp: traced 15 active commenters. Top overlaps: #ai-agents (67%), #devtools (47%), #llm (40%), #automation (33%). Cross-post to these tags to reach the same audience with zero extra effort.

---

**👤 You:**
> "Publish my article about MCP protocol layers on Dev.to with proper canonical URL."

**🤖 AI Agent:**
> Using `publish_article`: article created successfully. Title: 'Beyond APIs: Autonomous Agents Need a Protocol Layer'. URL: https://dev.to/username/beyond-apis-autonomous-agents-need-a-protocol-layer-3edj. Tags: mcp, ai-agents, devtools, automation. Canonical URL set to your original blog post.


## ❓ FAQ

**Q: Can this server post comments on Dev.to?**
No. The Forem API intentionally does not expose a comment creation endpoint as an anti-spam measure. This server provides full comment reading and analysis capabilities, but comment creation must be done manually through the Dev.to interface.

**Q: What makes the intelligence tools different from just reading the API?**
Each intelligence tool orchestrates 20-40 API calls and applies proprietary algorithms. For example, `audience_crossover` fetches top articles in a tag, extracts all commenters, then fetches each commenter's articles to map which other tags they write about — revealing hidden community overlaps that no single API call can surface.

**Q: Do I need an API key for all tools?**
Public read tools (search, get articles, get tags, get user) work without authentication. Authenticated tools (my articles, my drafts, publish, update, toggle reaction, followed tags, reading list, followers) require a Dev.to API key. Intelligence tools work without authentication but deliver richer results with one.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/devto-intelligence](https://vinkius.com/mcp/devto-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dev.to Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `devto-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dev.to Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "devto-intelligence": {
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
