# OpenAlex MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openalex-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Automate scholarly research via OpenAlex — search millions of works, authors, and institutions directly from any AI agent.

## Description
Connect to **OpenAlex**, the world's most comprehensive open index of the global research system. Empower your AI agent to navigate the vast landscape of scholarly knowledge through natural conversation.

### What you can do

- **Scholarly Works** — Search, filter, and retrieve metadata for millions of articles, books, and datasets using `list_works` and `get_work`.
- **Author Profiles** — Identify researchers, their affiliations, and impact metrics using `list_authors` and `get_author`.
- **Institutional Insights** — Explore universities and research organizations globally with `list_institutions` and `get_institution`.
- **Venues & Sources** — Inspect journals, conferences, and repositories via `list_sources` and `get_source`.
- **Discovery & Taxonomy** — Navigate topics, publishers, and funders to understand the funding and publication landscape using specialized listing tools.

### How it works

1. Subscribe to this server
2. (Optional) Enter your OpenAlex API Key for the 'Polite Pool' (faster limits)
3. Start querying the world's research from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Academics** — quickly find relevant literature and track citations without leaving your writing environment
- **Data Scientists** — gather bibliometric data and map research trends programmatically
- **Students** — discover authoritative sources and key authors for any field of study


## Available Tools (14)
- **get_author**: Get a single author by their OpenAlex ID
- **get_funder**: Get a single funder by its OpenAlex ID
- **get_institution**: Get a single institution by its OpenAlex ID
- **get_publisher**: Get a single publisher by its OpenAlex ID
- **get_source**: Get a single source by its OpenAlex ID
- **get_topic**: Get a single topic by its OpenAlex ID
- **get_work**: g., W2741809807).

Get a single scholarly work by its OpenAlex ID
- **list_authors**: Always resolve names to IDs here before filtering works.

List, search, or filter authors
- **list_funders**: List, search, or filter funders
- **list_institutions**: List, search, or filter institutions (universities, research orgs)
- **list_publishers**: List, search, or filter publishers
- **list_sources**: List, search, or filter sources (journals, repositories, conferences)
- **list_topics**: List, search, or filter research topics
- **list_works**: Supports search, filter (e.g., author.id:A123, publication_year:>2020), sort, and group_by.

List, search, or filter scholarly works (articles, books, datasets)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenAlex** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for scholarly works about 'Large Language Models' published in 2023."

**🤖 AI Agent:**
> I've found several highly cited works from 2023. Top results include 'Sparks of Artificial General Intelligence' and 'LLaMA: Open and Efficient Foundation Language Models'. Would you like the full metadata for any of these?

---

**👤 You:**
> "List the top 5 research institutions in Germany by works count."

**🤖 AI Agent:**
> Based on OpenAlex data, the top institutions in Germany are: 1. Helmholtz Association, 2. Max Planck Society, 3. University of Munich, 4. Heidelberg University, 5. Technical University of Munich. Would you like to explore the authors associated with any of these?

---

**👤 You:**
> "Get detailed information for author ID A5023888321."

**🤖 AI Agent:**
> Retrieving profile... This ID belongs to Yoshua Bengio. He has over 1,000 works indexed, with a high citation count in Computer Science and Artificial Intelligence. His primary affiliation is Université de Montréal.


## ❓ FAQ

**Q: How do I find works by a specific author if I only have their name?**
First, use `list_authors` with the `search` parameter to find the author's OpenAlex ID. Once you have the ID (e.g., A5012345678), use `list_works` with a filter like `author.id:A5012345678`.

**Q: Can I filter research papers by publication year or citation count?**
Yes. Use the `filter` parameter in `list_works`. For example, `publication_year:>2020` or `cited_by_count:>100`. You can also use the `sort` parameter like `cited_by_count:desc` to see the most impactful works first.

**Q: Is an API key mandatory to use this server?**
No. OpenAlex offers a free public tier. However, providing an API key places you in the 'Polite Pool', which offers faster rate limits and more consistent performance for heavy research tasks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openalex-alternative](https://vinkius.com/mcp/openalex-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenAlex** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `openalex-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenAlex** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "openalex-alternative": {
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
