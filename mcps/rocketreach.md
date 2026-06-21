# RocketReach MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rocketreach)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rocketreach-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rocketreach-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Find accurate contact information for professionals and companies with a database of verified emails and direct phone numbers.

## Description
Connect your **RocketReach** account to any AI agent and take full control of your B2B lead generation and contact enrichment orchestration through natural conversation. RocketReach provides a premier platform for finding verified emails and phone numbers, and this integration allows you to search for professionals, retrieve company metadata, and manage webhooks directly from your chat interface.

### What you can do

- **Lead & Person Orchestration** — Search for professionals by name, title, or company and retrieve detailed profile metadata programmatically.
- **Contact Enrichment Intelligence** — Perform instant lookups for specific individuals using RocketReach IDs or LinkedIn URLs to reveal verified contact info directly from the AI interface.
- **Company & Firmographic Control** — Search and retrieve detailed company profiles, including domains and employee counts via natural language.
- **Usage & Credit Oversight** — Access real-time account profile metadata and monitor credit usage to ensure your outreach campaigns are always optimized.
- **Operational Monitoring** — Track system activity, manage webhooks, and retrieve billing info using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your RocketReach API Key from your account settings
3. Start enriching your sales pipeline from Claude, Cursor, or any MCP-compatible client

No more manual LinkedIn scraping or credit wasting. Your AI acts as a dedicated sales development representative or lead analyst.

### Who is this for?

- **SDRs & Recruiters** — quickly retrieve verified contact info for target prospects without switching apps.
- **Marketing Teams** — automate the enrichment of lead lists and track search history via natural conversation.
- **Operations Teams** — streamline the retrieval of account statistics and monitor organizational credit health directly within the chat.


## Available Tools
- **check_lookup_status**: Check async lookup status
- **create_webhook**: complete.

Create a new webhook
- **delete_webhook**: Delete a webhook
- **get_account_info**: Get account profile
- **get_billing_info**: Get billing details
- **get_credit_usage**: Get credit usage stats
- **list_recent_searches**: List search history
- **list_webhooks**: List configured webhooks
- **lookup_company**: Get company details
- **lookup_person**: Consumes 1 credit.

Get verified contact info
- **search_companies**: Search for companies
- **search_people**: Search for professionals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RocketReach** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'John Doe' who works at 'Google'."

**🤖 AI Agent:**
> I've performed the search. I found a match for 'John Doe' (Lead Software Engineer) at Google. Would you like me to look up his verified contact information?

---

**👤 You:**
> "Search for VP of Engineering contacts at Series B SaaS companies in San Francisco."

**🤖 AI Agent:**
> Found 23 VP of Engineering profiles matching criteria. Top results: James Park (VP Engineering, CloudScale, 120 employees, Series B $24M). Email: j.park@cloudscale.io (verified). Sarah Chen (VP Engineering, DataForge, 85 employees, Series B $18M). Email: sarah@dataforge.com (verified). Alex Rivera (VP Platform Engineering, APIFirst, 200 employees, Series B $35M). Email: alex.r@apifirst.io (verified). 20 additional results available. Email accuracy: 94%. Phone numbers found for 18 of 23 contacts.

---

**👤 You:**
> "Look up the complete profile and contact information for the CEO of Meridian Corp."

**🤖 AI Agent:**
> Profile found: David Chen, CEO & Co-founder, Meridian Corp. Email: d.chen@meridiancorp.com (verified, last validated 3 days ago). Phone: +1-415-555-0198 (direct line). LinkedIn: linkedin.com/in/davidchen-meridian. Location: San Francisco, CA. Company: Meridian Corp (Enterprise SaaS, 340 employees, Series C $52M). Previous: CTO at DataFlow (2018-2021), Senior Engineer at Google (2014-2018). Education: Stanford CS MS, MIT BS. Board member: 2 advisory roles.


## Installation & Usage

To install and use the **RocketReach** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rocketreach](https://vinkius.com/mcp/rocketreach)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
