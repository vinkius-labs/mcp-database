# Double the Donation MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/double-the-donation)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/double-the-donation-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/double-the-donation-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Maximize nonprofit revenue by identifying donors whose employers offer matching gift programs and automating match requests.

## Description
Connect your **Double the Donation** (360MatchPro) account to any AI agent and take full control of your nonprofit matching gift automation and corporate giving workflows through natural conversation.

### What you can do

- **Employer Orchestration** — Search an extensive database of over 24,000 employers programmatically to find specific matching gift opportunities and guidelines
- **Donation Life-cycle** — Programmatically register new donations and automatically identify matching gift eligibility to maximize your fundraising revenue
- **Supporter Tracking** — Access complete status reports for individual donations and monitor the matching gift journey from donor action to payment completion
- **Account Management** — Programmatically provision and manage 360MatchPro accounts for nonprofit clients to streamline your partnership operations
- **Strategic Visibility** — Access high-level dashboard statistics and account settings directly through your agent for instant performance reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Public and Private API Keys** from your 360MatchPro dashboard (Settings > API Keys)
3. Start capturing unclaimed matching gift revenue from Claude, Cursor, or any MCP client

No more manual employer lookups or missing out on corporate gift matches. Your AI acts as your dedicated matching gift coordinator and fundraising strategist.

### Who is this for?

- **Nonprofit Development Teams** — instantly verify employer matching programs and register gifts using natural language commands
- **Fundraising Operations** — monitor donation status across your entire portfolio and track payment completion without leaving your workspace
- **Software Providers** — automate the provisioning of 360MatchPro accounts for your nonprofit clients through simple AI queries


## Available Tools
- **create_organization**: Provision a new 360MatchPro account
- **get_account_settings**: Get account settings
- **get_company**: Get company matching gift details
- **get_dashboard_stats**: Get dashboard statistics
- **get_donation**: Get donation details
- **get_organization**: Get organization details
- **list_campaigns**: List campaigns
- **list_donations**: List donations
- **list_subsidiaries**: List company subsidiaries
- **register_donation**: Register a new donation
- **search_company**: Search for a company by name
- **update_organization**: Update organization details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Double the Donation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Microsoft' in the employer matching database."

**🤖 AI Agent:**
> Searching database... I found 'Microsoft' (ID: 1024). They have a robust matching gift program with a 1:1 ratio up to $15,000 per employee. Would you like the full guidelines?

---

**👤 You:**
> "Register a $100 donation for 'john.doe@example.com'."

**🤖 AI Agent:**
> Donation registered! I've successfully sent the $100.00 gift from John Doe to 360MatchPro. I'll now monitor the matching eligibility and alert you if an employer is identified.

---

**👤 You:**
> "Get the current matching gift status for donation ID 'don_123'."

**🤖 AI Agent:**
> Fetching status... Donation don_123 is currently in the 'Waiting for Donor' stage. The donor has been notified to submit their matching request. Shall I check for any update emails sent?


## Installation & Usage

To install and use the **Double the Donation** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/double-the-donation](https://vinkius.com/mcp/double-the-donation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
