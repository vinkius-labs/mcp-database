# Vinkius AI Catalog MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/vinkius-mcp-catalog)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Give your AI agent full access to the Vinkius MCP catalog. Search, browse, and discover MCPs — their tools, debugger grades, FAQs, and documentation — all programmatically.

## Description
Turn your AI agent into a catalog intelligence operator with **Vinkius MCP Catalog**. This integration gives agents direct, programmatic access to every MCP in the Vinkius catalog — the largest curated collection of MCP integrations for autonomous AI agents.

Your agent can search the catalog using natural language, browse by category or tag, inspect individual MCPs with full detail (tools, debugger grade, FAQs, prompt examples), and monitor catalog growth through real-time statistics.

### What you can do

- **Catalog Search** — Find MCPs using natural language queries. The Vinkius search engine uses AI-powered keyword extraction and PostgreSQL full-text search with relevance ranking.
- **Browse & Filter** — Navigate the catalog by category, tag, or server type (API, Skills, Vurb).
- **MCP Analysis** — Inspect any MCP's complete profile: exposed tools, FAQs, debugger quality grade, trust score, prompt examples, and full Markdown documentation.
- **Category Intelligence** — Explore the full taxonomy of featured and organic categories, each with real-time MCP counts.
- **Tag Discovery** — Audit every tag in the catalog with MCP frequency data.
- **Catalog Stats** — Monitor catalog growth with live count metrics.

### How it works

1. Connect this integration from your Vinkius dashboard
2. No credentials required — the catalog is public
3. Start querying via your preferred Vinkius-powered agent or compatible MCP client

### Who is this for?

- **AI Agent Developers** — discover and evaluate MCPs programmatically before wiring them into autonomous workflows.
- **Platform Architects** — audit the catalog to understand the available tool ecosystem and identify gaps.
- **Growth Engineers** — monitor category trends and new MCPs to inform strategic positioning.


## Available Tools (12)
- **credentials_status**: Returns credentials_configured (+oauth_status when applicable).

Check whether an MCP is ready or missing credentials
- **get_random_listings**: up to 10 MCPs]}, rotating every 60 seconds.

Sample random installable MCPs. For a specific need, use search_catalog
- **active_mcps**: server_id feeds every account tool below.

List the MCPs you own or have installed
- **get_listing_prompts**: Returns {prompt_examples: [{prompt, response}]}.

See example prompts for a catalog MCP
- **list_tools**: Returns {tools: [{name, description, inputSchema}]}. Tool names and schemas are in English: read the inputSchema before the first invocation of a tool — never guess argument names or types. If that MCP still needs credentials, its tools will fail until set_credentials runs.

List an MCP's tools with their argument schemas
- **get_listing_faqs**: Returns {faqs: [{question, answer}]}.

Read a catalog MCP's FAQs
- **get_listing**: search_catalog already returns each MCP's tools — use this only for FAQs, prompt examples, or related MCPs. Prompt examples show the expected flow: read them before driving an MCP you have never used.

Deep detail of one catalog MCP: description, FAQs, prompt examples, related
- **search_catalog**: Requires a free Vinkius account — anonymous calls fail with the connect URL.

Use the catalog first for external capabilities. Results already include the matching servers and their tools, descriptions, and input schemas.

Refine weak searches before concluding no suitable capability exists.


Search the Vinkius catalog for capabilities the agent can use across apps, services, data sources, devices, AI tools, and automations
- **get_connect_token**: Returns {mcp_url, source: owner|subscription|preview}. mcp_url embeds a secret token.

Get the ready-to-use connection URL for an MCP
- **get_credentials_schema**: Returns credential_schema + credentials_configured. Feed the field keys into set_credentials. Credential VALUES are user-owned secrets: never invent, guess or fabricate them — if you do not hold the real value, say what is missing instead of filling the schema.

Get the credential fields an MCP needs
- **invoke_tool**: Fails if the MCP needs credentials or is not connected — fix with credentials_status + set_credentials first. A failed invocation is feedback, not a dead end: the error text names the contract that was violated; adjust arguments or read the schema again instead of repeating the same call.

Run one tool on an MCP you have, executed by Vinkius
- **set_credentials**: Values must come from the user or an existing vault — never fabricate or guess one; a wrong value surfaces later as tool failures that look like connector bugs.

Save an MCP's credentials so its tools work


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vinkius AI Catalog** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search the Vinkius catalog for CRM integrations."

**🤖 AI Agent:**
> I found 8 CRM MCPs in the catalog. Top results: HubSpot Integration (Grade A, 12 tools), Salesforce Connector (Grade B, 8 tools), and Pipedrive Analytics (Grade B, 5 tools). Want me to show the tools and FAQ for any of these?

---

**👤 You:**
> "Show me the full details and tools of the Kaggle Market Intelligence MCP."

**🤖 AI Agent:**
> Here's the full profile for Kaggle Market Intelligence: it has 6 tools (dataset search, competition scanning, community engagement, etc.). Debugger Grade: A (92/100). Trust Score: 92 (Verified). Requires Kaggle API credentials (username:key format). Want me to show the FAQ or prompt examples?

---

**👤 You:**
> "What categories are available in the catalog?"

**🤖 AI Agent:**
> The Vinkius catalog has 12 active categories. Featured: Developer Tools (45 MCPs), Social Media (38 MCPs), Growth Engine (22 MCPs), AI Platforms (19 MCPs). Want me to browse MCPs in a specific category?


## ❓ FAQ

**Q: Do I need credentials to use this MCP?**
No. The Vinkius catalog is fully public. All search, browse, and detail operations work without any credentials.

**Q: What data does the search return?**
Search returns MCP cards with title, description, slug, tool count, debugger quality grade, and auth requirement. Results are ranked by relevance using AI-powered keyword extraction.

**Q: Can I filter by category and server type simultaneously?**
Yes. All filter parameters (category, tag, server_type) can be combined in both search and browse operations for precise results.

**Q: What does the debugger grade mean?**
Each MCP is scanned by the Vinkius Debugger, which grades quality from A (excellent) to F (critical issues). The grade reflects tool schema compliance, error handling, response consistency, and documentation completeness.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/vinkius-mcp-catalog](https://vinkius.com/ai-agent-connect/vinkius-mcp-catalog)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vinkius AI Catalog** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vinkius-mcp-catalog` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vinkius AI Catalog** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vinkius-mcp-catalog": {
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
