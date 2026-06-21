# Clearbit (HubSpot) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clearbit-hubspot)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/clearbit-hubspot-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/clearbit-hubspot-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Enrich person and company data via Clearbit — track leads, monitor firmographics, and audit B2B intelligence directly from any AI agent.

## Description
Connect your **Clearbit (HubSpot)** account to any AI agent and take full control of your B2B intelligence through natural conversation. Streamline how you research prospects and companies natively.

### What you can do

- **Combined Enrichment** — Enrich both person and company data simultaneously using a single email address natively
- **Person Intelligence** — Access detailed professional information including job titles and social profiles flawlessly
- **Company Logistics** — Retrieve firmographic data such as industry, size, and location using domain names securely
- **Discovery Logistics** — Search for new companies based on specific criteria like technology stack or revenue flawlessly
- **Autocomplete Intelligence** — Suggest company names and domains based on partial queries flawlessly
- **Account Visibility** — Retrieve core account and quota information directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Clearbit API Key (obtained from your dashboard)
3. Start enriching your B2B data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Development (SDRs)** — research prospects and verify company details using natural language
- **Marketing Teams** — automate lead enrichment and segment audiences without opening the dashboard
- **Account Executives** — quickly look up stakeholder profiles and firmographics straight from their chat interface
- **Operations Teams** — verify API usage and monitor enrichment data quality


## Available Tools
- **find_person**: Find person by email
- **find_company**: Find company by domain
- **find_person_and_company**: Find person & company
- **autocomplete_company**: Autocomplete company
- **reveal_ip**: Reveal IP address
- **find_risk**: Calculate risk
- **get_prospects**: Get prospects
- **get_watchlist**: Get watchlist companies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clearbit (HubSpot)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Enrich this email address: alex@clearbit.com"

**🤖 AI Agent:**
> Enriching alex@clearbit.com... This is Alex MacCaw, Founder at Clearbit. He is based in San Francisco and has a background in software engineering. Would you like to see his social links?

---

**👤 You:**
> "Show me firmographic data for 'segment.com'."

**🤖 AI Agent:**
> Checking segment.com... Segment is a B2B SaaS company in the Analytics industry with over 500 employees and approximately $100M+ in revenue. They are based in San Francisco.

---

**👤 You:**
> "Find SaaS companies in California with 100-500 employees."

**🤖 AI Agent:**
> Searching Clearbit Discovery... I found several companies matching your criteria, including 'Vanta', 'Figma', and 'Honeycomb'. Would you like the full list or details for one of them?


## Installation & Usage

To install and use the **Clearbit (HubSpot)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clearbit-hubspot](https://vinkius.com/mcp/clearbit-hubspot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
