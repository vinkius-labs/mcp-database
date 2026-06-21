# AeroLeads MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aeroleads)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/aeroleads-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/aeroleads-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Find verified business emails and phone numbers for any prospect and build targeted lead lists in seconds.

## Description
Connect your **AeroLeads** account to any AI agent and take full control of your B2B lead generation and high-fidelity contact enrichment workflows through natural conversation.

### What you can do

- **Verified Email Orchestration** — Instantly find professional email addresses using prospect names and company domains with high-fidelity verification status
- **LinkedIn Enrichment Intelligence** — Programmatically retrieve over 60 data points from LinkedIn URLs, including verified phone numbers, job roles, and skills
- **Prospect Lifecycle Management** — List and manage your captured leads programmatically, or create new high-fidelity records directly through your agent
- **Domain Discovery Architecture** — Find all professional contacts associated with a specific company domain to identify key decision-makers programmatically
- **Operational Monitoring** — Track your remaining account credits and monitor team activity directly through your agent for instant performance reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your AeroLeads dashboard (Settings > API Key)
3. Start orchestrating your prospecting pipeline from Claude, Cursor, or any MCP client

No more manual toggling between browser extensions or guessing prospect emails. Your AI acts as your dedicated sales development representative and data architect.

### Who is this for?

- **SDRs & Recruiters** — instantly build high-fidelity prospect lists and enrich LinkedIn profiles using natural language commands
- **Marketing Managers** — automate lead generation for outreach campaigns and monitor account credits without leaving your workspace
- **Growth Leads** — integrate high-speed B2B contact data into custom data pipelines through simple AI queries


## Available Tools
- **add_new_lead**: Manually add lead
- **delete_lead**: Remove captured lead
- **search_domain_leads**: Find leads in domain
- **find_email_by_name**: Find email by name
- **get_account_info**: Get profile info
- **get_credit_balance**: Get credit status
- **get_lead_details**: Get full lead info
- **get_linkedin_details**: Enrich LinkedIn profile
- **list_captured_leads**: List your leads
- **list_prospecting_lists**: List lead lists
- **list_team_members**: List account users
- **list_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AeroLeads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the email for 'Elon Musk' at 'tesla.com'."

**🤖 AI Agent:**
> I've performed the high-fidelity search. I found a verified email for Elon Musk at tesla.com. This operation consumed 1 credit. Would you like to check his LinkedIn profile details?

---

**👤 You:**
> "Enrich the profile for this LinkedIn URL: 'https://linkedin.com/in/example'."

**🤖 AI Agent:**
> LinkedIn enrichment complete! I've retrieved high-fidelity data including her current role as 'CTO' and 2 verified phone numbers. Shall I add her as a new lead in your CRM list?

---

**👤 You:**
> "Search for all leads in the 'vinkius.com' domain."

**🤖 AI Agent:**
> Scanning domain... I found 5 professional contacts associated with vinkius.com, including the 'Head of Engineering' and 'CEO'. Would you like the detailed profile metadata for the CEO?


## Installation & Usage

To install and use the **AeroLeads** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aeroleads](https://vinkius.com/mcp/aeroleads)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
