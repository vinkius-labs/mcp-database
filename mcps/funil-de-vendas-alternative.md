# Funil de Vendas MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/funil-de-vendas-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage CRM opportunities, sales funnels, and activities via Funil de Vendas directly from your AI agent.

## Description
Empower your AI agent with access to your **Funil de Vendas** CRM to automate your sales pipeline and lead management workflows.

### What you can do

- **Opportunity Tracking**. List and search all sales deals across multiple funnels using filters like date and funnel ID.
- **Lead Generation**. Register new leads and opportunities directly into the CRM through automated data entry.
- **Activity Management**. Create, list, and update follow-up tasks, activities, and sales interactions.
- **CRM Oversight**. Access reference data like sales vendors, product catalogs, lead origins, and custom fields.

### How it works

1. Subscribe to this server
2. Enter your Funil de Vendas account Email and Password
3. Start managing your sales pipeline from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales Representatives**. Quickly log activities and check lead statuses via natural language commands.
- **Sales Managers**. Monitor team performance and pipeline health without leaving your workspace.
- **Marketing Teams**. Automate the creation of leads from various sources directly into the sales funnels.


## Available Tools (12)
- **check_crm_api_health**: Verify CRM API connectivity
- **create_crm_activity**: Requires opportunity ID and subject.

Add a new activity/follow-up
- **create_new_deal_lead**: Used for form integration.

Add a new lead/opportunity via Data Entry
- **list_crm_activities**: List CRM activities and tasks
- **list_crm_custom_fields**: List defined custom fields
- **list_sales_funnels**: List configured sales methodologies (funnels)
- **list_loss_motives**: List motives for losing deals
- **list_crm_opportunities**: Can be filtered by funnel code, date, or text search.

List CRM opportunities (deals)
- **list_lead_origins**: g., Google, Referral, Facebook).

List lead source origins
- **list_crm_products**: List registered products/services
- **list_sales_vendors**: List CRM users (vendors)
- **update_crm_activity**: Modify an existing activity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Funil de Vendas** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my active sales funnels in Funil de Vendas."

**🤖 AI Agent:**
> I've found 2 active sales funnels: 'Direct Sales' (ID: 101) and 'Referral Funnel' (ID: 102). Would you like to see opportunities from any of these?

---

**👤 You:**
> "Register a new lead: John Doe, john@example.com, subject 'Interested in Enterprise Plan'."

**🤖 AI Agent:**
> Done! I've registered John Doe as a new lead in your CRM with the subject 'Interested in Enterprise Plan'.

---

**👤 You:**
> "Show my recent follow-up activities."

**🤖 AI Agent:**
> I've retrieved your recent activities. You have 3 tasks completed and 2 upcoming follow-up calls scheduled for today.


## ❓ FAQ

**Q: Where do I get my login credentials?**
Use the same Email and Password you use to log in to your [**Funil de Vendas**](https://app.funildevendas.com.br/) account.

**Q: Can the agent move deals between stages?**
Yes, by using the `update_crm_activity` or lead entry tools, the agent can interact with the status and progress of your opportunities.

**Q: Is it possible to list all sales funnels?**
Absolutely. The `list_sales_funnels` tool retrieves all methodologies configured in your account along with their unique codes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/funil-de-vendas-alternative](https://vinkius.com/mcp/funil-de-vendas-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Funil de Vendas** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `funil-de-vendas-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Funil de Vendas** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "funil-de-vendas-alternative": {
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
