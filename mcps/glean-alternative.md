# Glean MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/glean-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search across all your company apps and docs with AI that understands your organization and surfaces the right answer instantly.

## Description
Connect your **Glean** workspace to any AI agent and unlock enterprise knowledge through natural conversation.

### What you can do

- **Universal Search** — Search across all connected data sources (Confluence, Slack, Google Drive, Jira, and more) from a single query
- **Datasource Filtering** — Focus searches on a specific connected platform for targeted results
- **People Search** — Find employees by name, role, expertise, or department across your organization
- **Document Management** — Index new documents, bulk-index batches, retrieve document metadata, and remove outdated content
- **Curated Collections** — Browse and inspect curated content collections for onboarding, policies, and shared knowledge
- **AI Chat** — Ask questions to Glean's AI assistant, which generates answers grounded in your organization's knowledge base
- **Autocomplete** — Get intelligent search suggestions based on organizational knowledge as you type

### How it works

1. Subscribe to this server
2. Enter your Glean API Token from the Admin Console
3. Start searching your enterprise knowledge from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Knowledge Workers** — find answers across Confluence, Slack, Drive, and Jira without switching between tools
- **IT Administrators** — index custom documents and manage curated collections programmatically
- **Engineering Teams** — search codebases, wikis, and design docs through a single conversational interface


## Available Tools (12)
- **autocomplete**: Autocomplete suggestions
- **bulk_index_documents**: Bulk index documents
- **chat**: AI chat
- **check_glean_status**: Verify connectivity
- **delete_document**: Delete a document
- **get_collection**: Get collection details
- **get_document**: Get document details
- **index_document**: Index a document
- **list_collections**: List collections
- **search_by_datasource**: g., Confluence, Slack, Google Drive).

Search in specific datasource
- **search_people**: Search people
- **search**: Search across all content


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Glean** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for our deployment runbook and the on-call rotation schedule."

**🤖 AI Agent:**
> Found 2 relevant results across your connected sources. 1) 'Production Deployment Runbook v3.2' — Confluence (Engineering wiki), last updated 3 days ago. Steps: pre-deploy checklist, rollback procedure, monitoring dashboards. 2) 'On-Call Rotation Q2 2025' — Google Sheets, shared by Sarah Chen. Current on-call: Mike Torres (Backend), Lisa Park (Frontend), expires May 2. Would you like to search for related incident reports or ask the AI assistant for a deployment summary?

---

**👤 You:**
> "Ask the AI assistant: What is our company's refund policy for enterprise customers?"

**🤖 AI Agent:**
> Based on your organization's knowledge base, the Glean AI assistant responds: 'Enterprise customers are eligible for a full refund within 30 days of contract signing. After 30 days, refunds are prorated based on remaining contract months. Refund requests must be submitted through the Customer Success team via Zendesk. All enterprise refunds require VP-level approval. Source: Customer Policy Handbook (Confluence, updated Feb 2025).' Would you like to see the full policy document or search for recent refund requests in Zendesk?

---

**👤 You:**
> "Find the engineering lead for the payments team and search Slack for recent discussions about PCI compliance."

**🤖 AI Agent:**
> People search result: James Rodriguez (james@company.com) — Senior Engineering Manager, Payments Team. Reports to: VP Engineering. Located: San Francisco. Expertise: payment processing, PCI-DSS, Stripe integration. Slack search results for 'PCI compliance': 3 relevant threads in #payments-eng. 1) 'PCI audit prep checklist' — 2 days ago, 12 replies. 2) 'TLS 1.3 migration timeline' — 5 days ago, 8 replies. 3) 'Tokenization vendor review' — 1 week ago, 15 replies. Would you like to read a specific thread or ask the AI for a PCI compliance summary?


## ❓ FAQ

**Q: Can I search across multiple data sources like Confluence, Slack, and Google Drive simultaneously?**
Yes! The `search` tool queries all connected data sources in a single request. If you want to narrow results to a specific platform, use `search_by_datasource` with the datasource name (e.g., 'Confluence', 'Slack', 'Google Drive'). Use `autocomplete` to get intelligent suggestions as you refine your query.

**Q: Can I ask the Glean AI assistant questions about my organization's knowledge?**
Yes. The `chat` tool sends a natural language question to Glean's AI assistant, which generates an answer grounded in your organization's indexed knowledge — including documents, wikis, Slack conversations, and Jira tickets. This is ideal for getting synthesized answers rather than just search results.

**Q: Can I index custom documents into Glean programmatically?**
Yes. Use `index_document` to add a single document with a JSON payload containing title, body, URL, and metadata. For large batches, use `bulk_index_documents` to index multiple documents in one request. Use `delete_document` to remove outdated content and `get_document` to verify indexing status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/glean-alternative](https://vinkius.com/mcp/glean-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Glean** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `glean-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Glean** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "glean-alternative": {
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
