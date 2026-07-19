# HubSpot CRM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hubspot-crm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Search, create, and manage HubSpot contacts, companies, notes, tasks, and associations through natural conversation.

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


## Available Tools (10)
- **hs_create_company**: The name is required. Providing the website domain (e.g., "acme.com") helps HubSpot auto-enrich the company with public data. Industry should match HubSpot industry categories. Returns the created company with its new HubSpot ID.

Create a new company record in HubSpot CRM with name, domain, industry, and phone
- **hs_create_note**: The body supports HTML. Notes appear in the timeline of associated records — essential for keeping CRM activity history. Provide contact, company, or deal IDs to link the note. Use to log meeting notes, call summaries, or internal context.

Create an engagement note in HubSpot attached to a contact, company, or deal for activity logging
- **hs_get_contact**: Returns full contact data including name, email, phone, company, lifecycle stage, lead status, last activity date, and all custom properties. Use after searching contacts to drill into a specific person for full details.

Get the complete details of a specific HubSpot contact by their record ID
- **hs_search_contacts**: Returns first name, last name, email, phone, associated company, lifecycle stage (subscriber/lead[REDACTED]), and assigned HubSpot owner. Use when the user wants to find a specific person, check contact details, verify lifecycle stage, or look up who is at a particular company.

Search HubSpot CRM contacts by name, email, phone, or company to find people in your database
- **hs_update_company**: Only specified fields are updated. Use when the user wants to update company details, correct industry classification, or change the domain.

Update properties of an existing HubSpot company by their record ID
- **hs_update_contact**: Only the fields you provide will be updated — other fields remain unchanged. Use when the user wants to correct contact info, update a phone number, change lifecycle stage, or reassign a contact.

Update properties of an existing HubSpot contact by their record ID
- **hs_create_contact**: Email is the primary deduplication key — if a contact with the same email already exists, the API will return an error. Provide first name, last name, phone, company name, and lifecycle stage to fully populate the record. Returns the created contact with its new HubSpot ID.

Create a new contact in HubSpot CRM with email as the unique identifier, plus name, phone, and company
- **hs_create_task**: Tasks appear in the tasks queue and can be assigned to owners. Set priority to HIGH, MEDIUM, or LOW. Due date should be ISO format. Associate with a contact by providing their ID. Use when the user wants to schedule follow-ups, create reminders, or assign action items.

Create a follow-up task in HubSpot with subject, due date, priority, and optional contact association
- **hs_get_associations**: For example: objectType="companies", objectId="123", toObjectType="contacts" returns all contacts associated with company 123. Common patterns: company→contacts, contact→deals, deal→contacts, contact→tickets. Use when the user asks "which contacts are at this company?" or "what deals does this contact have?"

Get associations between HubSpot CRM objects — e.g., find all contacts linked to a company, or deals linked to a contact
- **hs_search_companies**: Returns company name, website domain, industry, annual revenue, employee count, and assigned owner. Use when the user wants to find a specific company, look up organizational details, or check company-level CRM data.

Search HubSpot CRM companies by name, domain, or industry to find organizations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HubSpot CRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

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

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hubspot-crm](https://vinkius.com/mcp/hubspot-crm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HubSpot CRM** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hubspot-crm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HubSpot CRM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hubspot-crm": {
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
