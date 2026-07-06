# GoHighLevel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gohighlevel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Equip your AI agent with direct access to GoHighLevel — manage contacts, pipelines, and campaigns without opening the CRM dashboard.

## Description
Connect **GoHighLevel** to your AI agent and manage your all-in-one marketing and CRM platform conversationally.

### What you can do

- **Contact Management** — Search, create, and update contacts with custom fields, tags, and notes.
- **Pipeline Tracking** — List pipeline stages, move opportunities, and track deal values across your sales funnels.
- **Campaign Analytics** — Query email and SMS campaign performance, open rates, and click-through metrics.
- **Calendar & Appointments** — List upcoming appointments, check availability, and manage booking calendars.

### How it works

1. Subscribe to the GoHighLevel integration on the marketplace.
2. Get your API key from your sub-account (Settings → Business Profile → API Key section).
3. Ask your AI agent to manage contacts, track deals, or query campaign data.

### Who is this for?

- **Marketing Agencies** — Manage multiple client accounts, track campaign performance, and update CRM data from a single interface.
- **Sales Teams** — Move deals through pipelines, update contact records, and check appointment schedules instantly.
- **Business Owners** — Get a real-time snapshot of leads, deals, and campaign metrics without navigating the full CRM.


## Available Tools (10)
- **create_contact**: Create a new contact
- **list_opportunities**: List pipeline opportunities
- **list_pipelines**: List sales pipelines
- **list_calendars**: List booking calendars
- **list_conversations**: List recent conversations
- **send_message**: Send an SMS/email to a contact
- **list_campaigns**: List drip campaigns
- **list_contacts**: List all CRM contacts
- **list_forms**: List lead capture forms
- **get_contact**: Get contact details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GoHighLevel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the contact 'John Smith' in my CRM."

**🤖 AI Agent:**
> Found: John Smith (john@acmecorp.com). Phone: +1 555-0123. Tags: Hot Lead, Enterprise. Pipeline: Sales (stage: Proposal Sent). Last activity: 3 days ago.

---

**👤 You:**
> "How many deals are in the 'Proposal' stage right now?"

**🤖 AI Agent:**
> There are 8 deals in the 'Proposal' stage with a total pipeline value of $124,500. The largest is Acme Corp ($45,000) and the oldest has been there for 12 days.

---

**👤 You:**
> "What are my upcoming appointments today?"

**🤖 AI Agent:**
> You have 4 appointments today: Sarah Chen at 10:00 AM (Discovery Call), Mark Johnson at 1:00 PM (Demo), Emily Davis at 3:00 PM (Follow-up), and Alex Rivera at 4:30 PM (Onboarding).


## ❓ FAQ

**Q: How do I get my GoHighLevel API key?**
Log in to your GoHighLevel sub-account. Click **Settings** (bottom left corner). Navigate to **Business Profile**. Scroll down to the **API Key** section — your key will be displayed there, or click **Generate Key** if one hasn't been created. Copy the key and paste it below. Note: In newer accounts, you may see a **Private Integration** option instead — create one and use the generated token.

**Q: Can I manage multiple client accounts from one agent?**
Yes. Each GoHighLevel sub-account has its own API key. Configure separate integrations for each client account and your AI agent can switch between them — managing contacts, deals, and campaigns across your entire agency portfolio.

**Q: Can my AI agent move deals through pipeline stages?**
Yes. Your agent can list all pipeline stages, view deals in each stage, update deal values, and move opportunities between stages — giving your sales team a conversational way to manage their entire sales process.

**Q: Does this work with GoHighLevel's white-label versions?**
Yes. The API is the same regardless of whether you use GoHighLevel directly or through a white-label reseller. The API key from your sub-account works identically across all branded versions of the platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gohighlevel](https://vinkius.com/mcp/gohighlevel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GoHighLevel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gohighlevel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GoHighLevel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gohighlevel": {
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
