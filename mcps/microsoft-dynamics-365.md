# Microsoft Dynamics 365 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/microsoft-dynamics-365)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/microsoft-dynamics-365-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/microsoft-dynamics-365-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage accounts, opportunities, orders, and business processes on Microsoft Dynamics 365 — the unified CRM & ERP platform.

## Description
Connect your **Microsoft Dynamics 365** environment to any AI agent and manage your CRM and ERP operations through natural conversation.

### What you can do

- **Account Management** — Create, read, and update account records including contacts, addresses, and relationship hierarchies
- **Opportunity Pipeline** — Query open opportunities by stage, probability, and close date; update deal values and ownership
- **Sales Orders** — Create and manage sales orders, quotes, and invoices across your sales organization
- **Case Management** — Create support cases, track resolution progress, and manage SLA compliance
- **Financial Operations** — Query journal entries, G/L accounts, and financial dimensions (Business Central)
- **Custom Entities** — Access any Dataverse entity through the Web API, including custom tables and relationships
- **Business Process Flows** — Check active stages in business process flows and advance records through pipeline stages

### How it works

1. Subscribe to this server
2. Enter your Azure AD app credentials (Client ID, Client Secret, Tenant ID) and Dynamics 365 environment URL
3. Start managing CRM/ERP operations through Claude, Cursor, or any MCP-compatible client

The entire Microsoft ecosystem — from Teams to Power BI to LinkedIn Sales Navigator — feeds into Dynamics 365. Now your AI agent is part of that ecosystem.

### Who is this for?

- **Sales Representatives** — update opportunities, create quotes, and check pipeline status through chat
- **Customer Service Agents** — create and resolve cases without navigating the Dynamics UI
- **Finance Teams** — query financial data and journal entries across Business Central directly
- **CRM Administrators** — audit entity configurations and manage data integrity through conversation


## Available Tools
- **query_dataverse**: Common entity sets: accounts, contacts, opportunities, incidents (cases), leads, salesorders, invoices. Use OData filter syntax.

Query any Dataverse entity set
- **count_records**: Useful for dashboards without fetching full records.

Count records in a Dynamics 365 entity set
- **get_record**: Example: get_record("accounts", "00000000-0000-0000-0000-000000000001").

Get a specific Dynamics 365 record
- **create_record**: Provide field values as JSON. For lookups, use the @odata.bind format.

Create a new record in Dynamics 365
- **update_record**: Only specify the fields you want to change.

Update an existing Dynamics 365 record
- **delete_record**: This action is irreversible.

Delete a Dynamics 365 record
- **list_accounts**: Use filter to narrow results.

List Dynamics 365 accounts
- **list_opportunities**: Filter by stage, close date, or estimated value.

List sales opportunities
- **list_cases**: List support cases (incidents)
- **list_contacts**: List Dynamics 365 contacts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Microsoft Dynamics 365** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all opportunities closing this month with value above $100K."

**🤖 AI Agent:**
> Found 8 opportunities closing this month with value > $100K: 1. 'Enterprise Cloud Migration' — $450,000 (Stage: Negotiate, Probability: 85%), 2. 'Digital Transformation Q2' — $280,000 (Stage: Propose, Probability: 70%), and 6 more. Total pipeline value: $1,890,000. Want details on any deal?

---

**👤 You:**
> "Create a new support case for account 'Contoso Ltd' about a billing discrepancy."

**🤖 AI Agent:**
> Support case CAS-2026-12345 created successfully. Account: Contoso Ltd, Subject: 'Billing Discrepancy', Priority: High, Status: Active. The case has been assigned to the Billing Support queue. Would you like to attach any documents or add internal notes?

---

**👤 You:**
> "What's the total revenue from the EMEA region this quarter?"

**🤖 AI Agent:**
> EMEA Revenue (Q2 2026): Total closed-won revenue: €3,240,000 across 34 deals. Top contributors: 1. UK — €1,120,000 (15 deals), 2. Germany — €890,000 (8 deals), 3. France — €620,000 (6 deals). Quarter-over-quarter growth: +14.2%. Want a breakdown by product line?


## Installation & Usage

To install and use the **Microsoft Dynamics 365** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/microsoft-dynamics-365](https://vinkius.com/mcp/microsoft-dynamics-365)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
