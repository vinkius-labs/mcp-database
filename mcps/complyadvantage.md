# ComplyAdvantage MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/complyadvantage)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Automate AML and KYC compliance — screen entities, manage search history, and monitor risks directly from your AI agent.

## Description
Connect your **ComplyAdvantage** account to any AI agent to streamline your Anti-Money Laundering (AML) and Know Your Customer (KYC) workflows through natural conversation.

### What you can do

- **Entity Screening** — Create new searches for individuals or companies using `create_search` with customizable fuzziness and filters.
- **Search Management** — Retrieve detailed results with `get_search_details` or list previous search history using `list_searches`.
- **Risk Monitoring** — Start or stop ongoing monitoring for specific entities using `update_search_monitors` to stay updated on risk profile changes.
- **Case Collaboration** — Add internal notes with `create_comment` and update search statuses or assignees using `update_search`.
- **Whitelisting & Risk Levels** — Refine entity details and risk classifications directly through the `update_search_entities` tool.

### How it works

1. Subscribe to this server
2. Enter your ComplyAdvantage API Key
3. Start screening and managing compliance risks from Claude, Cursor, or any MCP client

### Who is this for?

- **Compliance Officers** — instantly screen new clients and manage alerts without switching between multiple dashboards.
- **Fintech Developers** — test and verify screening logic directly from the code editor or terminal.
- **Risk & Legal Teams** — automate the gathering of search details and audit trails for regulatory reporting.


## Available Tools (14)
- **delete_search_tag**: Detach tags from a search
- **get_search_details**: Get full search results
- **get_search_monitors**: Get monitored search details
- **get_search**: Get an overview of a search
- **list_comments**: Retrieve comments for a specific search
- **list_searches**: Get a list of previous searches
- **update_search_entities**: Update entity details (whitelist, risk level)
- **update_search_monitors**: g., start or stop).

Start/stop monitoring
- **update_search_profile**: Update the Search Profile for a monitored search
- **update_search**: Update search details (assignee, status)
- **list_users**: Get a list of users in your account
- **acknowledge_monitor**: Acknowledge changes to a monitored search
- **create_comment**: Create a comment on a search or entity
- **create_search**: ) with optional fuzziness and filters.

Create a new search


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ComplyAdvantage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for a person named 'John Smith' with a fuzziness of 0.7."

**🤖 AI Agent:**
> I've initiated the search for 'John Smith'. The search ID is 'SR-99283'. I found 3 potential matches. Would you like to see the full details for these results?

---

**👤 You:**
> "List the most recent searches performed in my account."

**🤖 AI Agent:**
> Retrieving your search history... Here are the last 5 searches: 'Acme Corp' (ID: 101), 'Jane Doe' (ID: 102), 'Global Tech' (ID: 103), etc. Which one would you like to inspect?

---

**👤 You:**
> "Add a comment to search ID 12345 saying 'Verified identity via passport'."

**🤖 AI Agent:**
> Comment successfully added to search 12345. The note 'Verified identity via passport' is now recorded in the case history.


## ❓ FAQ

**Q: How do I perform a new AML screening search for a company?**
Use the `create_search` tool. You can provide the company name in the `search_term` and optionally add `filters` like country codes or specific entity types to narrow down the results.

**Q: Can I enable ongoing monitoring for a specific search result?**
Yes. Use the `update_search_monitors` tool with the specific Search ID. This allows you to start or stop the monitoring service for that entity to receive updates on risk changes.

**Q: How can I see the full details and risk matches of a previous search?**
You can use `get_search_details` with the Search ID to retrieve the full detailed results, including all identified risk matches and entity metadata.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/complyadvantage](https://vinkius.com/mcp/complyadvantage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ComplyAdvantage** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `complyadvantage` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ComplyAdvantage** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "complyadvantage": {
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
