# Evvnt Marketing & Distribution MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/evvnt-marketing-distribution)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to manage events, track syndication reports, and monitor distribution via the Evvnt API.

## Description
Integrate **Evvnt**, the leading event marketing and distribution platform, directly into your AI workflow. Manage your event listings and categories, track real-time syndication reports and site reach, monitor saved venues and partner networks, and oversee your event promotion using natural language.

### What you can do

- **Event Oversight** — List and retrieve detailed information, categories, and status for all your promoted events.
- **Distribution Intelligence** — Monitor syndication reports, resolving total sites reached, clicks, and real-time distribution telemetry.
- **Network Management** — Access and monitor the Evvnt syndication partner network and saved venue profiles.
- **Marketing Auditing** — Retrieve high-level summaries of event volume, distribution success, and organizational account health instantly.

### How it works

1. Connect the Evvnt integration to your AI assistant.
2. Authorize using your Evvnt Partner API Key (found in your account settings).
3. Orchestrate your event promotion and distribution strategy through intuitive conversation.

### Who is this for?

- **Event Marketers** — Quickly check distribution reports and site reach on the go.
- **Venue Managers** — Research saved venue details and event statuses via chat.
- **Operations Teams** — Monitor syndication activity and organizational account metadata instantly.


## Available Tools
- **get_evvnt_account_metadata**: Retrieve metadata and limits for your Evvnt account
- **get_event_distribution_reports**: Get distribution and performance reports for a specific event
- **get_event_detailed_data**: Get detailed settings and distribution information for a specific event
- **quick_event_marketing_audit**: Retrieve a high-level summary of events and distribution reach
- **list_event_categories**: List all event categories supported by Evvnt
- **list_marketing_events**: List all events managed in your Evvnt account
- **list_syndication_partners**: List all syndication partners and sites in the Evvnt network
- **list_draft_marketing_events**: Identify events that are currently in a "Draft" or "Pending" status
- **list_successfully_distributed_events**: Identify events that have been successfully distributed to the partner network
- **list_saved_venues**: List all saved venues and locations in your account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Evvnt Marketing & Distribution** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active event marketing campaigns."

**🤖 AI Agent:**
> I've found 5 active campaigns, including 'Summer Jazz Festival' and 'Tech Innovation Workshop'. Both are currently 'Published' and distributed to the network. Would you like to see the distribution report for the Jazz Festival?

---

**👤 You:**
> "Show me the distribution report for event ID '12345'."

**🤖 AI Agent:**
> For event ID '12345', I've retrieved the report: 450 total sites reached, 1,230 clicks generated, and active syndication on top partner sites. Should I pull the geographic reach summary?

---

**👤 You:**
> "Check saved venues in our account."

**🤖 AI Agent:**
> You have 12 saved venues, including 'The Grand Theater', 'City Convention Center', and 'Downtown Gallery'. All profiles are active. Would you like the contact details for The Grand Theater?


## ❓ FAQ

**Q: How do I get an Evvnt API Key?**
Log in to your Evvnt partner dashboard, navigate to **Account > API**, and you can generate or retrieve your unique **Partner API Token** from there. API access is typically provided to authorized partners.

**Q: Does the integration show clicks per site?**
Yes, you can use the get_event_distribution_reports tool to retrieve detailed telemetry, including total site count and engagement metrics for specific events.

**Q: Can the agent submit new events?**
This integration currently focuses on listing and auditing promoted events and reports. Submitting new events for syndication should be managed via the Evvnt submission interface or automated ingestion partner tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/evvnt-marketing-distribution](https://vinkius.com/mcp/evvnt-marketing-distribution)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Evvnt Marketing & Distribution** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `evvnt-marketing-distribution` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Evvnt Marketing & Distribution** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "evvnt-marketing-distribution": {
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
