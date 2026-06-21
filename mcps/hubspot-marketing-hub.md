# HubSpot Marketing Hub MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hubspot-marketing-hub)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage marketing emails, forms, contact lists, campaigns, and landing pages through natural conversation.

## Description
Connect **HubSpot CRM** to any AI agent — instant access to your full CRM data without switching tabs.

### What you can do
- **Contacts** — Search, create, and manage contacts
- **Companies** — Find companies by name or domain
- **Deals** — Search and create deals with pipeline tracking
- **Tickets** — Create and search support tickets
- **Notes** — Create notes attached to any CRM record
- **Owners** — View all owners and team assignments
- **Pipelines** — List deal and ticket pipeline stages

### Who is this for?
- **Sales Reps** — Manage your CRM without leaving your AI assistant
- **Support Teams** — Create tickets and notes on-the-go
- **RevOps** — Pipeline snapshots and owner assignments
- **Managers** — Full CRM visibility through conversation


## Available Tools (6)
- **hs_form_submissions**: Returns each submission with the field values the visitor entered, submission date, and page URL. Use when the user wants to review lead capture data, check who submitted a form, or analyze form conversion data. You need the form ID — use hs_list_forms to find it.

Get individual form submissions for a specific HubSpot form, showing submitted field values and dates
- **hs_list_campaigns**: Returns campaign name, type, current state, and associated dates. Campaigns group related marketing assets (emails, landing pages, ads) under a single initiative for unified tracking. Use when the user asks about marketing initiatives, campaign performance, or wants to review active campaigns.

List marketing campaigns in HubSpot with name, type, status, and campaign dates
- **hs_list_contact_lists**: Returns list name, type (STATIC for manual lists, DYNAMIC for smart lists with auto-updating criteria), and count of contacts in each list. Use when the user asks about audience segments, marketing lists, wants to know list sizes, or needs to understand audience targeting.

List HubSpot contact lists (static and smart/dynamic) with name, type, and contact count
- **hs_list_forms**: Returns form name, form type (regular/popup/embedded), number of fields, and submission count. Forms are the primary lead capture mechanism in HubSpot. Use when the user asks about lead generation forms, wants to audit form performance, or needs a form ID to check submissions.

List HubSpot forms used for lead capture with name, type, field count, and submission volume
- **hs_list_landing_pages**: Returns page title, publish status (draft/published), URL slug, and full public URL. Landing pages are standalone pages designed for conversion (form fills, downloads). Use when the user asks about landing pages, lead capture pages, or wants to review publishing status.

List HubSpot landing pages with title, publish status, URL slug, and full page URL
- **hs_list_marketing_emails**: Returns email name, subject line, type (regular/automated/blog), current state (draft/published/sent), and publish/send date. Use when the user asks about email campaigns, wants to see recent sends, or needs to check which emails are active.

List marketing emails in HubSpot with name, subject line, send status, type, and publish date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HubSpot Marketing Hub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for contacts at Acme Corp"

**🤖 AI Agent:**
> 👥 **Contacts at Acme Corp**
| Name | Email | Phone | Lifecycle |
|---|---|---|---|
| John Smith | john@acme.com | +1 555-0123 | Customer |
| Sarah Chen | sarah@acme.com | +1 555-0456 | Lead |

---

**👤 You:**
> "Create a deal: Enterprise Package $50,000"

**🤖 AI Agent:**
> ✅ **Deal Created!**
- Name: Enterprise Package
- Amount: $50,000
- Pipeline: Sales Pipeline
- Stage: Appointment Scheduled

---

**👤 You:**
> "Show me the deal pipeline stages"

**🤖 AI Agent:**
> 📊 **Sales Pipeline**
1. Appointment Scheduled
2. Qualified to Buy
3. Presentation Scheduled
4. Decision Maker Bought-In
5. Contract Sent
6. Closed Won ✅
7. Closed Lost ❌


## ❓ FAQ

**Q: What HubSpot data can I access?**
Contacts, Companies, Deals, Tickets, Notes, Owners, and Pipelines. All data respects your HubSpot permissions.

**Q: Can I create and update records?**
Yes! Create contacts, deals, tickets, and notes. All through natural conversation.

**Q: How does authentication work?**
Uses a HubSpot Private App token (Bearer). Create a Private App in Settings > Integrations > Private Apps, copy the token, and paste it.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hubspot-marketing-hub](https://vinkius.com/mcp/hubspot-marketing-hub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HubSpot Marketing Hub** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hubspot-marketing-hub` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HubSpot Marketing Hub** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hubspot-marketing-hub": {
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
