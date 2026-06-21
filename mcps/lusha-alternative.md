# Lusha MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lusha-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lusha-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lusha-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Enrich your prospect data with verified direct dials and email addresses from a B2B contact intelligence platform.

## Description
Connect your **Lusha** account to any AI agent and take full control of your sales prospecting and data enrichment through natural conversation. Lusha provides a premier B2B database, and this integration allows you to retrieve high-fidelity contact details (email, phone), enrich company metadata, and search for new prospects directly from your chat interface.

### What you can do

- **Contact & Person Enrichment** — Lookup detailed contact metadata programmatically using name, company, or LinkedIn URLs to ensure your CRM is always synchronized.
- **Company & Firmographic Intelligence** — Access and monitor company data including industry, revenue, and headcount directly from the AI interface to qualify accounts in real-time.
- **Prospecting & Search Control** — Search for new contacts and companies matching your Ideal Customer Profile (ICP) via natural language to drive better sales efficiency.
- **Usage & Credit Oversight** — Access granular details for your credit consumption and remaining balance using simple AI commands to maintain a clear overview of your resources.
- **Operational Monitoring** — Track system responses and manage data ingestion to ensure your sales workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Lusha API Key from your dashboard settings
3. Start enriching your sales data from Claude, Cursor, or any MCP-compatible client

No more manual copy-pasting from LinkedIn profiles. Your AI acts as a dedicated sales researcher or lead qualification assistant.

### Who is this for?

- **Sales Development Reps (SDRs)** — quickly retrieve phone numbers and monitor account health without switching apps.
- **Account Executives** — automate the enrichment of new leads and track prospecting progress via natural conversation.
- **Marketing Teams** — streamline the retrieval of firmographic metadata and monitor data quality directly within the chat.


## Available Tools
- **bulk_enrich_companies**: Enrich multiple companies
- **bulk_enrich_persons**: Enrich multiple contacts
- **enrich_company_info**: Get firmographics
- **enrich_person_info**: Get contact details
- **get_credit_balance**: Check account balance
- **get_person_by_email**: Enrich by email
- **get_person_by_linkedin**: Enrich by LinkedIn
- **get_usage_stats**: Check API usage
- **get_account_info**: Check connection
- **prospect_new_companies**: Search for businesses
- **prospect_new_leads**: Search for contacts
- **test_lusha_auth**: Verify API key


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lusha** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Enrich this contact: John Miller at Acme Corp."

**🤖 AI Agent:**
> I've enriched the contact. John Miller is the 'VP of Sales' at Acme Corp. His verified email is j.miller@acme.com and I've also found a direct office number.

---

**👤 You:**
> "Search for companies in New York with 500-1000 employees in the SaaS industry."

**🤖 AI Agent:**
> I've found 12 companies matching your criteria, including 'CloudStream' and 'DataVibe'. Would you like me to retrieve the LinkedIn URLs for their decision-makers?

---

**👤 You:**
> "Check my Lusha credit balance."

**🤖 AI Agent:**
> You currently have 450 credits remaining in your monthly plan. Your next renewal is in 12 days.


## Installation & Usage

To install and use the **Lusha** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lusha-alternative](https://vinkius.com/mcp/lusha-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
