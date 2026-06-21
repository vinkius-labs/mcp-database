# HubSpot Operations Hub MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hubspot-operations-hub)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage workflows, CRM properties, pipelines, owners, and property groups through natural conversation.

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
- **hs_create_property**: Create a custom property (field) on a HubSpot CRM object to extend the data model with business-specific fields
- **hs_list_all_pipelines**: Returns pipeline name, stage labels, internal stage IDs, and display order. Pipelines define the process stages for deals (sales process) or tickets (support process). Use when configuring automations, setting up deal/ticket routing, or when the user needs pipeline/stage IDs for creating records.

List all deal or ticket pipelines with their stages, IDs, and display order for workflow configuration
- **hs_list_owners**: Owners are the users who can be assigned to contacts, companies, deals, and tickets. Returns owner ID, name, email, active status, and team memberships. Use when configuring round-robin assignment rules, auditing user access, or when the user needs owner IDs for record assignment.

List all HubSpot owners (CRM users) for use in assignment workflows, with name, email, and active status
- **hs_list_properties**: Returns property internal name, display label, data type (string/number/date/enumeration), field type (text/number/date/select/checkbox), group name, and description. Essential for understanding the CRM data model. Use when the user asks "what fields exist on contacts?", wants to audit custom properties, or needs internal property names for filters/searches.

List all properties (fields) configured on a HubSpot CRM object type — contacts, companies, deals, or tickets
- **hs_list_property_groups**: Returns group internal name and display label. Property groups organize fields into logical sections in the HubSpot UI (e.g., "Contact Information", "Social Media", "Custom Fields"). Use to find valid group names before creating custom properties with hs_create_property.

List property groups for a HubSpot CRM object — the logical sections that organize properties in the UI
- **hs_list_workflows**: Returns workflow name, type (drip/standard/nurturing), enabled status (active vs inactive), and number of actions in the workflow. Workflows automate marketing, sales, and service processes — e.g., lead nurturing emails, deal stage automation, ticket routing. Use when the user asks about active automations, wants to audit workflows, or needs to check which automations are running.

List all automation workflows in HubSpot with name, type, active/inactive status, and action count


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HubSpot Operations Hub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

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

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hubspot-operations-hub](https://vinkius.com/mcp/hubspot-operations-hub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HubSpot Operations Hub** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hubspot-operations-hub` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HubSpot Operations Hub** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hubspot-operations-hub": {
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
