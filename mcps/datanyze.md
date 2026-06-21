# Datanyze MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/datanyze)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/datanyze-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/datanyze-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Equip your AI agent to retrieve B2B lead intelligence, technographics, and company insights via the Datanyze API.

## Description
Integrate **Datanyze**, the leader in technographics and B2B intelligence, directly into your AI workflow. Research target companies, identify the software technologies they use, and retrieve contact information for key decision-makers using natural language.

### What you can do

- **Technographic Auditing** — Identify the CMS, CRM, marketing automation, and other technologies used by any domain.
- **Lead Generation** — Search for B2B companies by industry or keyword and retrieve contact profiles.
- **Market Analysis** — Find domains similar to your competitors and track global traffic ranks.
- **Credit Monitoring** — Keep track of your Datanyze API credit balance directly via chat.

### How it works

1. Connect the Datanyze integration to your AI assistant.
2. Authorize using your Datanyze API Token and account Email.
3. Empower your sales and marketing research through intuitive conversation.

### Who is this for?

- **Sales Development Reps (SDRs)** — Quickly research a prospect's tech stack before outreach.
- **Marketing Teams** — Identify target segments based on technology usage and industry sector.
- **Business Analysts** — Gather data on market competitors and traffic trends via chat.


## Available Tools
- **get_domain_contacts**: Resolves individual profiles including job titles, departments, and professional social links for identified decision-makers.

List key decision-makers and contact profiles for a domain
- **get_api_credit_balance**: Check your remaining Datanyze API credits
- **get_domain_intelligence**: Returns a comprehensive profile including active software stacks, website metadata, and organizational technographic attributes.

Retrieve technographics and metadata for a specific domain
- **quick_tech_audit**: Identify core technologies used by a domain
- **get_domain_traffic_rank**: Retrieve the global traffic rank for a specific domain
- **list_technology_customers**: Returns a list of company domains currently identified as users of the specified platform.

List companies currently using a specific technology ID
- **list_industry_sectors**: List all industry categories available for filtering
- **list_competitor_domains**: Returns a list of domains sharing similar technographic profiles or industry characteristics.

Find domains similar to or competing with a specific domain
- **list_tracked_technologies**: Returns a list of technical identifiers and category classifications for various software solutions.

List all software technologies and platforms tracked by Datanyze
- **search_b2b_companies**: Matches query terms against company names, industry sectors, and descriptive metadata to return a list of matching organizational entities.

Search for companies matching a specific keyword or industry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Datanyze** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What technologies are used by 'stripe.com'?"

**🤖 AI Agent:**
> Stripe.com uses several core technologies, including AWS for infrastructure, Google Analytics for tracking, and Salesforce for CRM. Would you like a full list of detected software?

---

**👤 You:**
> "Find B2B companies in the 'Fintech' industry in London."

**🤖 AI Agent:**
> I've found several Fintech companies in London, including 'Monzo', 'Revolut', and 'Starling Bank'. Should I retrieve the contact details for the decision-makers at any of these companies?

---

**👤 You:**
> "How many API credits do I have left?"

**🤖 AI Agent:**
> You currently have 450 credits remaining in your Datanyze account for the current billing cycle. Would you like to see a summary of your recent usage?


## Installation & Usage

To install and use the **Datanyze** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datanyze](https://vinkius.com/mcp/datanyze)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
