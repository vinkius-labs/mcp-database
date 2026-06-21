# Findymail MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/findymail)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/findymail-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/findymail-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Find and verify verified B2B emails and direct phone numbers using natural language agents.

## Description
Connect your **Findymail** account to any AI agent and supercharge your sales prospecting and data enrichment workflows through the power of the Model Context Protocol (MCP). Findymail is designed for high-growth sales teams that need accurate, verified contact data without the manual grind of searching through LinkedIn or guessing email patterns.

### What you can do

- **Precision Email Finding** — Instantly retrieve verified B2B emails by providing a person's name and their company domain or name. No more guessing; get data that actually delivers.
- **Real-time Email Verification** — Protect your sender reputation by verifying any email address before it hits your outreach sequence. Our verification tool checks for deliverability in seconds.
- **Direct Phone Discovery** — Scale your cold calling efforts by fetching direct phone numbers directly from LinkedIn profiles using our specialized phone finder tool.
- **Deep Company Enrichment** — Transform a simple domain or LinkedIn URL into a full company profile, including industry data, size, and social identifiers.
- **Intellimatch Lead Generation** — Use natural language to discover new leads. Simply ask your agent to 'Find SaaS founders in the US' or 'Get me marketing heads in London', and let Findymail do the heavy lifting.
- **List & Contact Management** — Organically manage your prospecting lists and retrieve specific contact details to keep your CRM updated and your outreach personalized.
- **Credit Monitoring** — Keep a pulse on your API usage with built-in tools to check your remaining credits and usage summaries directly from your AI conversation.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Findymail API Token (found in your dashboard settings)
3. Start managing your lead generation directly from Claude, Cursor, or any MCP-compatible environment

### Who is this for?

- **SDRs & BDRs** — find the right contacts for your target accounts without leaving your AI assistant, saving hours of manual data entry.
- **Marketing Operations** — ensure your lead lists are clean, verified, and enriched with the latest metadata before launching major campaigns.
- **Founders & Recruiters** — quickly identify and reach out to key decision-makers or potential candidates with verified direct contact information.


## Available Tools
- **create_contact_list**: Create a new contact list
- **enrich_company**: Enrich company data
- **find_email**: Find a verified email address
- **find_phone**: Find direct phone numbers
- **get_contact**: Get contact details
- **get_credits_summary**: Get credits usage summary
- **get_credits**: Check credit balance
- **get_lead_search_data**: Get lead search results
- **get_lead_search_status**: Check lead search status
- **list_contact_lists**: List all contact lists
- **search_leads**: Find companies and contacts
- **verify_email**: Verify an email address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Findymail** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the verified email for Satya Nadella at microsoft.com"

**🤖 AI Agent:**
> Searching... I found a verified email for Satya Nadella at Microsoft. The email is verified and safe to send.

---

**👤 You:**
> "Enrich company data for the domain 'vinkius.com'"

**🤖 AI Agent:**
> Fetching data... I've retrieved the company profile for Vinkius, including LinkedIn URL, industry, and size metrics.

---

**👤 You:**
> "Search for 'marketing agency owners in New York' using Intellimatch."

**🤖 AI Agent:**
> Lead search task started! The Task ID is 'task_123'. I will check the status and notify you when the results are ready to be fetched.


## Installation & Usage

To install and use the **Findymail** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/findymail](https://vinkius.com/mcp/findymail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
