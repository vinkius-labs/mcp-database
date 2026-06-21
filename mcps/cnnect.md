# Cnnect MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cnnect)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cnnect-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cnnect-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Streamline business networking with digital business cards, contact management, and relationship tracking for professionals.

## Description
Connect your **Cnnect.nl** NFC business card account to any AI agent and take full control of your professional networking and lead generation workflows through natural conversation.

### What you can do

- **Digital Profile Orchestration** — Retrieve and update your digital business card contact details, branding, and social links to maintain a high-fidelity professional identity
- **Lead Generation Intelligence** — List and manage leads captured programmatically via your physical NFC cards or digital profile visits to streamline your sales pipeline
- **NFC Asset Management** — Access your directory of physical NFC cards and monitor their individual status and usage metadata directly through your agent
- **Networking Analytics** — Access comprehensive usage summaries and detailed click analytics to understand how your profile is being engaged with in real-time
- **Team Visibility** — Retrieve directories of company members and monitor account-level settings to perfectly coordinate organization-wide digital networking

### How it works

1. Subscribe to this server
2. Retrieve your **API Bearer Token** from your Cnnect Business Portal (Settings > API)
3. Start managing your professional network from Claude, Cursor, or any MCP client

No more manual entry of paper business cards. Your AI acts as your dedicated networking associate and CRM ingestion coordinator.

### Who is this for?

- **Sales Professionals** — instantly retrieve new leads captured during networking events using natural language commands
- **Business Owners** — monitor company-wide networking performance and manage member profiles without leaving your workspace
- **Marketing Teams** — track profile engagement and click-through rates across digital assets through simple AI queries


## Available Tools
- **get_analytics_summary**: Get overall usage analytics
- **get_click_analytics**: Get detailed click analytics
- **create_lead**: Manually create a new lead
- **get_card_details**: Get details for a specific NFC card
- **get_lead_details**: Get details for a specific lead
- **get_my_profile**: Get your Cnnect profile data
- **get_account_settings**: Get Cnnect account settings
- **list_physical_cards**: List your physical NFC cards
- **list_leads**: List leads captured via your card
- **list_company_members**: List company team members
- **list_tags**: List lead tags
- **update_profile**: Update your digital business card profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cnnect** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my digital business card profile and social links."

**🤖 AI Agent:**
> I've retrieved your profile. You are currently listed as 'John Doe' (Architect). Your digital card includes links to LinkedIn and your personal site. Would you like to update any of your contact metadata?

---

**👤 You:**
> "List the last 5 leads captured via my NFC card."

**🤖 AI Agent:**
> Fetching leads... I found 5 recent contacts, including 'Alice Brown' and 'TechCorp Sales'. I've retrieved their emails and phone numbers. Shall I add them to your main project tracker?

---

**👤 You:**
> "What is my overall networking performance for this month?"

**🤖 AI Agent:**
> Scanning analytics... Your card has been tapped 150 times this month with a 30% lead conversion rate. Engagement is up by 15% compared to last month. Would you like a breakdown of clicks by social platform?


## Installation & Usage

To install and use the **Cnnect** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cnnect](https://vinkius.com/mcp/cnnect)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
