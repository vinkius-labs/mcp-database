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
- **get_listing_prompts**: ].

Call this to see example prompts for a catalog MCP and understand what it does
- **search_catalog**: Omit query to browse. Every result is an MCP addressed by its slug — call get_listing with that slug to inspect it. For a logged-in user who already has a result MCP, that result carries a server_id (UUID) usable directly with invoke_tool and get_connect_token; server_id is null otherwise. Results never expose an internal listing id — the catalog is addressed only by slug.

When you do not have a tool or connector for the user's request, call this to search the catalog and find one. Never tell the user something is impossible before searching here
- **get_credentials_schema**: Returns credential_schema (field keys, types, required) and credentials_configured. Build the set_credentials payload from these keys. Secrets are never returned.

Call this to get the credential fields a connector needs before its tools can be used, then pass them to set_credentials
- **get_random_listings**: ]}.

Call this to sample random catalog MCPs and discover connectors you did not know existed. For a specific need, use search_catalog instead
- **set_credentials**: Handles both owned and installed MCPs.

Call this to save a connector's credentials so its tools become usable. Call get_credentials_schema first for the required fields
- **credentials_status**: Returns credentials_configured (boolean) and oauth_status when applicable. For the field keys, use get_credentials_schema.

Call this to check whether a connector is ready to use or still needs credentials
- **get_listing_faqs**: ].

Call this to read the FAQs of a catalog MCP you are evaluating
- **list_tools**: Returns { server_id, name, requires_auth, tools: [{name, description, inputSchema}] }. If requires_auth is true, the MCP still needs credentials before its tools will work.

Call this to get the tools of an MCP the user has, with their names and argument schemas, before running one with invoke_tool
- **get_listing**: Returns the MCP detail, its full tool list, FAQs, category listings and related MCPs. installed/authenticated/ready are booleans for the current user (null if anonymous). If the user is logged in and has this MCP, the response also carries a server_id (UUID) you can use directly with invoke_tool and get_connect_token; server_id is null when the user is anonymous or does not have this MCP yet.

After search_catalog returns a match, call this to inspect that MCP and confirm it has the tools you need before telling the user to install it
- **get_connect_token**: Returns { mcp_url, source } where source is owner | subscription | preview. The mcp_url embeds the connection token — treat it as a secret. Reuses the user's existing token when one exists, otherwise mints one.

Call this to get the connection URL for an MCP so a client can connect to it. Returns a ready-to-use mcp_url with the token embedded
- **invoke_tool**: Returns the tool result. Fails if the MCP is not connected for execution or still needs credentials — use credentials_status and set_credentials to fix that first.

Call this to run a tool on an MCP the user already has, without connecting to it yourself. Vinkius runs it on the user's behalf and returns the result. Get the tool name and argument schema from list_tools first
- **active_mcps**: Narrow with filter (active|inactive), search (by name) or page.

Call this to list the connectors the user already has. If none matches the task, call search_catalog to find a new one. Use it to get the server_id needed by list_tools, invoke_tool, get_credentials_schema, credentials_status, set_credentials and get_connect_token


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
