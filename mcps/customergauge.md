# CustomerGauge MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/customergauge)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/customergauge-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/customergauge-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Equip your AI agent to manage B2B experience, monitor NPS scores, and track revenue impact directly via the CustomerGauge API.

## Description
Integrate **CustomerGauge**, the leading B2B Experience Management platform, directly into your AI workflow. Monitor customer survey responses, track Net Promoter Scores (NPS) across your account portfolio, and analyze the revenue impact of customer experience using natural language.

### What you can do

- **Response Monitoring** — List and retrieve full details for customer survey responses and feedback.
- **Account NPS Tracking** — Monitor NPS metrics for specific business accounts and business units.
- **Contact Insights** — Access detailed profiles and survey history for individual account contacts.
- **Revenue Impact Analysis** — List revenue data associated with accounts to understand experience-driven growth.

### How it works

1. Connect the CustomerGauge integration to your AI assistant.
2. Authorize using your CustomerGauge API Key.
3. Orchestrate your B2B experience strategy through intuitive conversation.

### Who is this for?

- **Account Managers** — Quickly check account NPS and recent feedback before client meetings.
- **Customer Success Teams** — Monitor survey responses and identify accounts at risk via chat.
- **Experience Analysts** — Gather structured data on revenue impact and B2B engagement for reporting.


## Available Tools
- **get_account_nps**: Resolves quantitative satisfaction scores. Interacts with the sentiment aggregation engine.

Get the Net Promoter Score (NPS) for a specific account
- **get_business_unit_nps**: Resolves organizational performance data. Interacts with the business unit hierarchy.

Get NPS metrics for a specific business unit
- **get_contact_profile**: Resolves interaction history and individual sentiment trends. Interacts with the customer lifecycle boundary.

Get detailed profile and survey history for a contact
- **get_portfolio_nps_summary**: Resolves global experience metrics. Touches the executive reporting boundary.

Get an overall NPS summary across your entire account portfolio
- **get_response_details**: Resolves verbatim comments, respondent metadata, and driver scores. Touches the granular feedback analytics boundary.

Get full details for a specific survey response
- **list_b2b_accounts**: Resolves account IDs, names, and organizational mappings. Touches the account management and segmentation boundary.

List all business accounts managed in CustomerGauge
- **list_account_contacts**: Resolves contact identifiers and associated account links. Touches the CRM and relationship boundary.

List contacts associated with your business accounts
- **list_survey_responses**: Resolves response IDs, scores (NPS), and timestamp data. Interacts with the survey response repository.

List all customer survey responses in CustomerGauge
- **list_revenue_impact_data**: Resolves monetary values and account associations for ROI calculation. Touches the financial data integration boundary.

List revenue data associated with accounts for experience impact analysis
- **search_responses_by_keyword**: Resolves feedback entries matching the query keyword. Touches the indexed text search boundary.

Search through survey comments and feedback by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CustomerGauge** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all survey responses received this morning."

**🤖 AI Agent:**
> I've found 5 new survey responses from this morning. Highlights include a score of 10 from 'TechCorp' and an 8 from 'Global Logistics'. Would you like to read the comments for any of these?

---

**👤 You:**
> "What is the current NPS for account 'Global Logistics'?"

**🤖 AI Agent:**
> The account 'Global Logistics' (ID: 123) has a current NPS of 45, based on 12 responses this year. This is a slight increase from last year's score of 42. Should I show you the most recent feedback from this account?

---

**👤 You:**
> "Search for feedback containing the word 'pricing'."

**🤖 AI Agent:**
> I found 3 responses containing 'pricing'. One customer mentioned that 'the pricing model is confusing for larger teams'. Would you like to see the details for these responses?


## Installation & Usage

To install and use the **CustomerGauge** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/customergauge](https://vinkius.com/mcp/customergauge)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
