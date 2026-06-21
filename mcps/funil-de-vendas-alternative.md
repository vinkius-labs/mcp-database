# Funil de Vendas MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/funil-de-vendas-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/funil-de-vendas-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/funil-de-vendas-alternative-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Funil de Vendas** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/funil-de-vendas-alternative](https://vinkius.com/mcp/funil-de-vendas-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
