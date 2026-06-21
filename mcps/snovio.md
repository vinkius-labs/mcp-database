# Snov.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/snovio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/snovio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/snovio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Equip your AI agent with direct access to Snov.io — find emails, verify addresses, automate drip campaigns, and manage prospect lists without opening the Snov dashboard.

## Description
Connect **Snov.io** to your AI agent and manage your email finder, verifier, and drip campaign platform conversationally.

### What you can do

- **Email Finder** — Find professional emails by domain, name, or company with confidence scores.
- **Email Verifier** — Validate email addresses before outreach to protect your sender reputation.
- **Drip Campaigns** — Create and manage automated email drip sequences with follow-ups.
- **Prospect Lists** — Build, manage, and export prospect lists with verified contact data.

### How it works

1. Subscribe to the Snov.io integration on the marketplace.
2. Get your API credentials from your Snov.io account (Profile → API tab → copy User ID and API Secret).
3. Ask your AI agent to find emails, verify addresses, or manage campaigns.

### Who is this for?

- **SDR Teams** — Find and verify decision-maker emails before starting outreach sequences.
- **Growth Teams** — Build targeted prospect lists by domain and automate initial outreach.
- **Freelancers & Agencies** — Cost-effective email finding and verification for smaller outreach operations.


## Available Tools
- **domain_search**: Domain email search
- **email_finder**: Find email
- **email_verifier**: Verify emails
- **add_prospect**: io list.

Add prospect
- **list_prospect_lists**: List prospect lists
- **get_prospect_by_email**: Get prospect
- **get_balance**: io credits.

Get credit balance
- **tech_checker**: Check domain technologies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Snov.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all emails at shopify.com."

**🤖 AI Agent:**
> Found 156 email addresses at shopify.com. Email pattern: {first}.{last}@shopify.com. Top results include contacts from Engineering, Marketing, and Sales departments. Credits used: 1.

---

**👤 You:**
> "Verify if alex@oldcompany.com is still deliverable."

**🤖 AI Agent:**
> Verification result: INVALID. Reason: mailbox does not exist (SMTP check returned 550 error). Recommendation: remove from your outreach list to protect sender reputation.

---

**👤 You:**
> "Find the email for Sarah Kim at Notion."

**🤖 AI Agent:**
> Found: sarah.kim@makenotion.com (confidence: 88%). Domain pattern: {first}.{last}@makenotion.com. Verification: valid (SMTP confirmed). Credits used: 1.


## Installation & Usage

To install and use the **Snov.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/snovio](https://vinkius.com/mcp/snovio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
