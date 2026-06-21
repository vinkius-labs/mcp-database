# FirstQuadrant MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/firstquadrant)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Let AI handle your outbound sales prospecting with autonomous research, personalized messaging, and smart follow-up sequences.

## Description
Connect your **FirstQuadrant** account to any AI agent and take full control of your B2B sales pipeline and contact enrichment workflows through natural conversation.

### What you can do

- **Lead Orchestration** — List and manage your complete database of leads and contacts, including retrieving detailed metadata and performing search lookups programmatically
- **AI Enrichment** — Trigger autonomous AI workflows to gather deep context about a lead from external sources and update contact profiles automatically
- **Campaign Management** — Access available sales sequences and enroll contacts into personalized email campaigns directly through your agent
- **Schema Intelligence** — Explore and manage your custom property schema to ensure all sales data is perfectly structured for AI analysis
- **Activity Monitoring** — Monitor the complete log of sales activities, including emails, calls, and AI-driven tasks in real-time

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** and **Organization ID** from FirstQuadrant (Settings > Developer Settings)
3. Start managing your B2B sales pipeline from Claude, Cursor, or any MCP client

No more manual contact research or complex campaign toggling. Your AI acts as your dedicated sales operations coordinator.

### Who is this for?

- **Sales Development Reps (SDRs)** — instantly identify top leads and trigger enrichment workflows using natural language
- **Account Managers** — retrieve full interaction histories and verify contact details without leaving your workspace
- **Growth Teams** — automate lead discovery and scale personalized outreach through simple AI queries


## Available Tools
- **add_to_campaign**: Add contact to a campaign
- **create_contact**: Create a new lead/contact
- **enrich_contact_ai**: Trigger AI enrichment for a contact
- **get_contact_details**: Get contact profile details
- **list_activities**: List sales activities
- **list_campaigns**: List sales campaigns/sequences
- **list_contacts**: Supports advanced filtering by email or created date.

List FirstQuadrant contacts
- **list_properties_schema**: List custom properties schema


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FirstQuadrant** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all qualified leads from FirstQuadrant."

**🤖 AI Agent:**
> I've retrieved your leads. You have 12 qualified contacts, including 'John Doe' (ID: 101) and 'Sarah Smith' (ID: 102). Would you like to see the interaction history for any of them?

---

**👤 You:**
> "Enrich the contact with email 'ceo@acme.com'."

**🤖 AI Agent:**
> AI enrichment triggered! I've started the research workflow for ceo@acme.com. I'll notify you as soon as the company size and latest funding details are added to the profile.

---

**👤 You:**
> "Add contact '101' to the 'Discovery Sequence'."

**🤖 AI Agent:**
> Contact enrolled! I've successfully added John Doe (ID: 101) to your 'Discovery Sequence'. They will receive the first automated email shortly.


## ❓ FAQ

**Q: How do I find my Organization ID in FirstQuadrant?**
Log in to your FirstQuadrant dashboard and navigate to **Settings** > **Developer Settings**. Your unique Organization ID will be listed there.

**Q: Can the agent update custom properties?**
Yes! Use the `create_contact` or `enrich_contact_ai` tools to manage standard and custom data points defined in your property schema.

**Q: How does AI enrichment work through the agent?**
The `enrich_contact_ai` tool triggers FirstQuadrant's autonomous research engine to scan public sources and update the contact record with high-fidelity insights.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/firstquadrant](https://vinkius.com/mcp/firstquadrant)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FirstQuadrant** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `firstquadrant` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FirstQuadrant** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "firstquadrant": {
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
