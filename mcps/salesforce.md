# Salesforce MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/salesforce)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Connect your Salesforce CRM to any AI agent — query records with SOQL, manage accounts, contacts, opportunities, run reports, and perform CRUD operations.

## Description
Connect your **Salesforce** CRM to any AI agent and manage your entire sales pipeline through natural conversation.

### What you can do

- **SOQL Queries** — Execute any SOQL query to retrieve data across all objects
- **Account Management** — List, view, create, and update accounts
- **Contact & Lead Management** — Browse contacts, search across all objects
- **Opportunity Tracking** — Monitor pipeline, create and update deals
- **Reports** — List and execute Salesforce reports
- **Full CRUD** — Create, read, update, and delete any SObject type
- **Global Search** — Full-text search across all Salesforce data


## Available Tools (12)
- **list_contacts**: List Salesforce contacts
- **list_opportunities**: List sales opportunities
- **get_record**: Specify the SObject type (Account, Contact, Opportunity, Case, Lead) and the record ID.

Get a specific Salesforce record by type and ID
- **soql_query**: Example: SELECT Id, Name FROM Account WHERE Industry = 'Technology' LIMIT 10

Execute a SOQL query against Salesforce
- **describe_object**: Useful for understanding data structure.

Get metadata about a Salesforce object
- **list_reports**: List available Salesforce reports
- **run_report**: Use list_reports first to find the report ID.

Execute a Salesforce report and get results
- **global_search**: Returns matches across Accounts, Contacts, Leads, and other objects simultaneously.

Search across all Salesforce objects
- **list_accounts**: List Salesforce accounts
- **create_record**: Provide JSON fields as a string.

Create a new Salesforce record
- **update_record**: Provide the SObject type, ID, and JSON fields to update.

Update an existing Salesforce record
- **delete_record**: This action is irreversible.

Delete a Salesforce record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salesforce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all open opportunities worth over $50,000."

**🤖 AI Agent:**
> Found 7 open opportunities over $50,000:

1. **Acme Corp - Enterprise License** — $120,000 (Stage: Negotiation)
2. **TechStart - Platform Migration** — $85,000 (Stage: Proposal)
3. **GlobalRetail - API Integration** — $67,500 (Stage: Discovery)
...

Total pipeline value: $487,500

---

**👤 You:**
> "Create a new lead for John Smith from TechCo, email john@techco.com."

**🤖 AI Agent:**
> ✅ Lead created successfully!

- **Name**: John Smith
- **Company**: TechCo
- **Email**: john@techco.com
- **ID**: 00Q8Z00001kL2mN
- **Status**: Open - Not Contacted

---

**👤 You:**
> "Run the Monthly Sales Report."

**🤖 AI Agent:**
> 📊 Monthly Sales Report (March 2026):

| Metric | Value |
|--------|-------|
| Total Revenue | $2.4M |
| Deals Closed | 34 |
| Avg Deal Size | $70,588 |
| Win Rate | 28% |
| Pipeline Growth | +15% |

Top performer: Sarah Chen ($485K closed)


## ❓ FAQ

**Q: Can I run custom SOQL queries?**
Yes! The `soql_query` tool accepts any valid SOQL string. Example: SELECT Id, Name, Amount FROM Opportunity WHERE StageName = 'Closed Won' LIMIT 20.

**Q: Can I create records in any object?**
Yes! Use `create_record` with the SObject type (Account, Contact, Lead, etc.) and a JSON string of fields.

**Q: How do I search across all Salesforce data?**
Use `global_search` with your search text. It uses SOSL to find matches across Accounts, Contacts, Leads, and all other objects simultaneously.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salesforce](https://vinkius.com/mcp/salesforce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salesforce** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `salesforce` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salesforce** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salesforce": {
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
