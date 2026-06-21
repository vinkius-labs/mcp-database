# ContactOut MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/contactout)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/contactout-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/contactout-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Find personal emails and direct phone numbers for professionals on LinkedIn to build targeted outreach lists that convert.

## Description
Connect your **ContactOut** account to any AI agent to streamline your B2B lead generation and talent acquisition workflows through natural conversation. ContactOut provides a powerful intelligence layer for discovering verified contact information and enriching professional profiles at scale.

### What you can do

- **Contact Discovery Orchestration** — Instantly retrieve verified email addresses and direct phone numbers using LinkedIn profile URLs programmatically
- **Professional Enrichment** — Enrich contact and company data with detailed attributes, including job titles, locations, and social links to maintain a high-fidelity CRM
- **Deep Semantic Search** — Programmatically search the ContactOut database of 300M+ people using advanced filters for skills, titles, and locations
- **Identity Resolution** — Find the LinkedIn profile associated with a specific email address to perfectly coordinate your multichannel outreach
- **Administrative Visibility** — Programmatically track your credit balance and API usage statistics to coordinate your recruitment and sales budgets

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your ContactOut dashboard (Settings > API)
3. Start finding decision-makers and enriching your lead lists from Claude, Cursor, or any MCP client

No more manual profile scraping or guessing email formats. Your AI acts as your dedicated sales associate and recruitment coordinator.

### Who is this for?

- **Sales Development (SDRs)** — build highly targeted outreach lists with verified contact info using natural language commands
- **Technical Recruiters** — search for candidates with specific skills and retrieve contact details without leaving your workspace
- **Growth Marketers** — automate lead enrichment and identify LinkedIn profiles from email lists through simple AI queries


## Available Tools
- **enrich_company**: Enrich company data
- **enrich_contact**: Enrich contact data
- **find_email_by_linkedin**: Find email by LinkedIn profile
- **find_linkedin_by_email**: Find LinkedIn profile by email
- **get_api_usage**: Get API usage statistics
- **search_companies**: Search for companies
- **search_people**: Search for people


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ContactOut** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the contact email for this LinkedIn profile: https://www.linkedin.com/in/williamhgates"

**🤖 AI Agent:**
> I've retrieved the contact details for William Gates. His verified email is 'bill@microsoft.com' and I've also found a direct phone line. Would you like the full professional enrichment data for this profile?

---

**👤 You:**
> "Search for 'Python' developers in 'London' with at least 5 years of experience."

**🤖 AI Agent:**
> Searching database... I found 15 matches for Python developers in London matching your criteria. Highlights include senior profiles at 'DeepMind' and 'Revolut'. Shall I retrieve the contact info for the top 3?

---

**👤 You:**
> "Check my current API credit balance on ContactOut."

**🤖 AI Agent:**
> Scanning account... You currently have 1,240 credits remaining in your account. Your connection is active and healthy. Need help enriching another lead list?


## Installation & Usage

To install and use the **ContactOut** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/contactout](https://vinkius.com/mcp/contactout)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
