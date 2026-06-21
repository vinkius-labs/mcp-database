# The Guardian MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/the-guardian)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access The Guardian's entire content archive — search articles, browse sections, explore tags, and retrieve full-text stories directly from any AI agent.

## Description
Connect to **The Guardian Open Platform** and unlock programmatic access to one of the world's most respected newsrooms through natural conversation.

### What you can do

- **Content Search** — Run full-text queries across the entire Guardian archive with filters by section, tag, date range, and custom ordering
- **Article Retrieval** — Fetch the complete body text, byline, publication date, and editorial metadata for any individual article
- **Section Browsing** — List all editorial sections (e.g. Technology, Politics, Sport) and browse their latest or most-viewed content
- **Tag Discovery** — Explore the taxonomy of keywords, contributors, series, and tones used to categorize Guardian journalism
- **Regional Editions** — Query content across UK, US, Australia, and International editions
- **Date-Range Research** — Retrieve articles published within specific time windows for historical analysis or event tracking

### How it works

1. Subscribe to this server
2. Register for a free API key at the Guardian Open Platform
3. Start querying world-class journalism from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Analysts** — pull structured data from decades of reporting for trend analysis, sentiment studies, or media monitoring
- **Journalists & Editors** — quickly surface related coverage, verify publication history, and retrieve source material without leaving the writing environment
- **Developers & Data Scientists** — integrate Guardian content pipelines into NLP workflows, dashboards, or knowledge bases


## Available Tools
- **get_item**: g. "world/2026/apr/08/example-article").

Get the full content of a specific Guardian article or item
- **get_latest_content**: Ordered by most recent first.

Get the most recent articles from The Guardian
- **get_section_details**: Get editorial highlights and most-viewed content for a section
- **list_editions**: List available Guardian regional editions
- **list_sections**: g. technology, politics, sport). Optionally filter by name.

List all editorial sections available on The Guardian
- **list_tags**: Filter by query, section, or tag type (keyword, series, contributor, tone, type, blog).

List tags used to categorize Guardian content
- **search_by_date_range**: Useful for historical research or tracking recent events.

Search Guardian content within a specific date range
- **search_by_section**: g. "technology", "world", "sport"). Supports pagination and ordering.

Browse content within a specific Guardian section
- **search_by_tag**: g. "technology/artificial-intelligence", "tone/features"). Supports pagination.

Browse content tagged with a specific Guardian tag
- **search_content**: Supports filtering by section, tag, date range, ordering, and pagination.

Search articles and content on The Guardian


## 💬 Prompt Examples

Here are some examples of how you can interact with the **The Guardian** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search The Guardian for recent articles about artificial intelligence in the technology section."

**🤖 AI Agent:**
> I found 10 recent articles in the Technology section matching 'artificial intelligence'. The most recent is 'AI reshapes the newsroom: how machine learning is transforming editorial workflows' published today by Alex Hern. Would you like to read the full article?

---

**👤 You:**
> "What are the main editorial sections available on The Guardian?"

**🤖 AI Agent:**
> The Guardian is organized into 48 editorial sections. The major ones include: World News, UK News, Politics, Business, Technology, Science, Sport, Culture, Opinion, and Environment. Would you like to browse the latest articles from any of these sections?

---

**👤 You:**
> "Find all Guardian articles about climate change published between January and March 2026."

**🤖 AI Agent:**
> I retrieved 47 articles mentioning 'climate change' published between 2026-01-01 and 2026-03-31. Key pieces include investigative reports on carbon markets, policy analysis from COP summits, and feature stories on climate migration. The most discussed article had 312 comments. Shall I fetch the full text of any specific article?


## ❓ FAQ

**Q: Can I retrieve the full text of a Guardian article, not just the headline?**
Yes. Use the `get_item` tool with the article's path ID. The response includes the full body text, byline, standfirst, publication date, section, tags, and thumbnail image when available.

**Q: How far back does the Guardian Content API archive go?**
The Guardian Content API provides access to articles dating back to 1999. You can use `search_by_date_range` with specific start and end dates to query historical content from any period covered by the archive.

**Q: Is a paid subscription required to use this integration?**
No. The Guardian Open Platform offers a free developer API key that supports up to 12 calls per second and 5,000 calls per day. This is sufficient for most research and automation workflows.

**Q: Can I filter articles by topic, section, or contributor?**
Yes. The `search_content` tool accepts section, tag, and date filters. Use `list_sections` to discover available sections and `list_tags` to find keywords, contributors, and series to refine your queries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/the-guardian](https://vinkius.com/mcp/the-guardian)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **The Guardian** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `the-guardian` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **The Guardian** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "the-guardian": {
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
