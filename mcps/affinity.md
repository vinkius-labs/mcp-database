# Affinity MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/affinity)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Relationship intelligence and CRM — manage lists, contacts, and interactions via AI.

## Description
Connect your **Affinity** account to your AI agent to unlock professional relationship intelligence and CRM orchestration. From auditing your smart lists to monitoring recent email and meeting interactions and managing your contact pipeline, your agent handles your deal flow through natural conversation.

### What you can do

- **Smart List Management** — List and retrieve entries for your custom smart lists, including statuses and field values
- **Relationship Intelligence** — Access relationship strength scores and identify 'warm' introduction paths within your network
- **Contact Oversight** — List and manage people and organizations, ensuring your B2B intelligence is always up-to-date
- **Interaction Auditing** — Retrieve logs of recent emails, meetings, and calls automatically synced from team accounts
- **Pipeline Insights** — Quickly identify active opportunities and track deal progress directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Affinity API Key
3. Start managing your relationships and monitoring your deal flow through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Venture Capital & Private Equity** — automate deal tracking and monitor relationship strength with portfolio founders
- **Sales & BD Professionals** — research contacts and audit recent interactions before outreach
- **Investor Relations** — manage investor lists and track engagement patterns effortlessly
- **Executive Assistants** — quickly look up organization details and update person records using simple commands


## Available Tools
- **list_persons**: Retrieve a paginated list of people your team has interacted with in your Affinity network
- **list_organizations**: Retrieve companies and institutions mapped within your Affinity CRM
- **list_smart_lists**: Retrieve the catalog of custom smart lists (pipelines) securely configured in your account
- **list_list_entries**: Retrieve the people or organizations associated with a specific Affinity smart list ID
- **list_interactions**: Retrieve recent chronological logs of synced emails, meetings, and calls across your team


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Affinity** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for a person contact with the name 'Jane Smith'."

**🤖 AI Agent:**
> I've found one person matching 'Jane Smith'. She is currently at 'Innovate Corp' and has a relationship strength of 85 with your team. Would you like to see her recent interactions?

---

**👤 You:**
> "List all entries in my 'Active Deals' smart list."

**🤖 AI Agent:**
> I've retrieved your 'Active Deals' list. There are currently 12 opportunities, including 'Series A - FutureTech' and 'Acquisition - AlphaSoft'. Would you like to check the latest status for any of them?

---

**👤 You:**
> "Show me the last 5 meetings my team had with 'Innovate Corp'."

**🤖 AI Agent:**
> I've retrieved the interaction logs for Innovate Corp. Your team had 5 meetings in the last two weeks, discussing partnership terms and product integration. Would you like the detailed notes for the most recent meeting?


## ❓ FAQ

**Q: How do I find my Affinity API Key?**
Log in to Affinity, go to **Settings** > **API Keys**. You can generate or copy your existing API key from there. Ensure you are on a supported plan (Scale or higher).

**Q: What is a Relationship Strength score?**
It is a numeric value from 0 to 100 calculated by Affinity based on your team's communication history. A higher score indicates more frequent and recent interactions.

**Q: Can I retrieve meeting logs via the agent?**
Yes! Use the `list_interactions` tool to see recent emails and meetings that have been automatically synced to your Affinity account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/affinity](https://vinkius.com/mcp/affinity)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Affinity** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `affinity` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Affinity** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "affinity": {
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
