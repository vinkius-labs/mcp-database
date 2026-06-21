# ZoomInfo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoominfo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zoominfo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zoominfo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Equip your AI agent with direct access to ZoomInfo — search company and contact records, enrich lead data, and build prospect lists without opening the ZoomInfo platform.

## Description
Connect **ZoomInfo** to your AI agent and access the world's largest B2B contact and company intelligence database conversationally.

### What you can do

- **Contact Search** — Find decision-makers by job title, seniority level, department, company, and location.
- **Company Intelligence** — Pull firmographic data including revenue, employee count, industry, and technology stack.
- **Data Enrichment** — Enrich existing CRM records with ZoomInfo's verified contact and company data.
- **Intent Data** — Identify companies showing buying signals and research intent for your product category.

### How it works

1. Subscribe to the ZoomInfo integration on the marketplace.
2. Generate API credentials from your ZoomInfo admin panel (Admin → API → Generate Credentials).
3. Ask your AI agent to search contacts, pull company intelligence, or enrich lead data.

### Who is this for?

- **Enterprise Sales Teams** — Find the right decision-makers at target accounts with verified emails and direct dials.
- **Revenue Operations** — Enrich CRM data at scale and maintain clean, up-to-date contact records.
- **Marketing Teams** — Build targeted account lists based on firmographic criteria and buying intent signals.


## Available Tools
- **search_contacts**: Search contacts
- **search_companies**: Search companies
- **enrich_contact**: Enrich contact
- **enrich_company**: Enrich company
- **get_usage**: Get API usage
- **list_intent_topics**: List intent topics
- **search_intent**: Search intent signals
- **get_company_news**: Get company news


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ZoomInfo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find CTOs at SaaS companies with 50-200 employees in San Francisco."

**🤖 AI Agent:**
> Found 34 CTOs matching your criteria. Top 3: Alex Kim (CTO at DataPipeline, 120 employees, $18M ARR), Maria Santos (CTO at CloudSync, 85 employees, $12M ARR), and James Lee (CTO at APIStack, 62 employees, $8M ARR). All have verified emails and direct dials.

---

**👤 You:**
> "Enrich the contact record for sarah@acme.com."

**🤖 AI Agent:**
> Enrichment complete for sarah@acme.com: Sarah Williams, VP of Sales at Acme Corp. Direct dial: +1-555-0199. LinkedIn: linkedin.com/in/sarahwilliams. Company: Acme Corp ($45M revenue, 320 employees, Series C, SaaS/Enterprise Software). Tech stack: Salesforce, HubSpot, Outreach.

---

**👤 You:**
> "Which companies are showing buying intent for 'marketing automation'?"

**🤖 AI Agent:**
> 12 companies in your target market are showing strong intent signals for 'marketing automation' this week: TechFlow Inc (intent score: 95), GrowthStack (89), DataDriven Co (87), and 9 others. Average company size: 200-500 employees.


## Installation & Usage

To install and use the **ZoomInfo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoominfo](https://vinkius.com/mcp/zoominfo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
