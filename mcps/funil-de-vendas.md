# Funil de Vendas MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/funil-de-vendas)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/funil-de-vendas-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/funil-de-vendas-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Visualize your sales funnel, track deal stages, and manage your pipeline with a CRM designed for the Brazilian market.

## Description
Connect your **Funil de Vendas** account to any AI agent and take full control of your sales methodology and CRM workflows through natural conversation.

### What you can do

- **Opportunity Orchestration** — List and manage sales deals programmatically, including retrieving detailed metadata and updating statuses across different methodologies
- **Relationship Management** — Create and manage contact profiles for both individuals and companies to maintain a high-fidelity CRM database
- **Methodology Intelligence** — Access your configured sales funnels and stages to coordinate complex deal cycles and ensure process adherence
- **Performance Insights** — Retrieve aggregate metrics and statistics for your contacts and sales pipeline directly through your agent
- **CRM Customization** — Explore and manage custom fields to store industry-specific data points for every opportunity and contact in your account

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** and **Email** from your Funil de Vendas dashboard
3. Start managing your sales opportunities from Claude, Cursor, or any MCP client

No more manual deal logging or digging through CRM menus. Your AI acts as your dedicated sales coordinator and CRM assistant.

### Who is this for?

- **Sales Representatives** — instantly register new leads and update opportunity statuses using natural language commands
- **Sales Managers** — monitor pipeline health and team performance through automated queries and reporting
- **Entrepreneurs** — manage customer relationships and track business growth without leaving your creative workspace


## Available Tools
- **create_company**: Create a new company
- **create_opportunity**: Create a new opportunity
- **create_person**: Create a new person
- **get_account_info**: Get CRM account details
- **get_opportunity**: Get opportunity details
- **get_people_stats**: Get people statistics
- **list_companies**: List registered companies
- **list_custom_fields**: List custom fields
- **list_funnels**: List sales methodologies/funnels
- **list_opportunities**: List all sales opportunities
- **list_people**: List registered people
- **update_opportunity**: Update an existing opportunity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Funil de Vendas** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current sales opportunities in Funil de Vendas."

**🤖 AI Agent:**
> I've retrieved your active opportunities. You have 4 deals in progress, including 'Software Implementation' ($5,000) and 'Training Pack' ($1,200). Which one would you like to update?

---

**👤 You:**
> "Create a new opportunity 'Cloud Migration' with a value of 10000."

**🤖 AI Agent:**
> Opportunity created! 'Cloud Migration' has been added to your primary funnel with a value of $10,000. I've assigned it the ID 'opp_123'. Shall I add a contact to this deal?

---

**👤 You:**
> "Show me the list of available sales funnels."

**🤖 AI Agent:**
> Retrieving methodologies... You have 2 active funnels: 'Standard Sales Process' and 'Inbound Leads'. Each has its own stages and conversion tracking. Which one should we analyze?


## Installation & Usage

To install and use the **Funil de Vendas** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/funil-de-vendas](https://vinkius.com/mcp/funil-de-vendas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
