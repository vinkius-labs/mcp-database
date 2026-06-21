# FunnelCockpit MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/funnelcockpit)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/funnelcockpit-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/funnelcockpit-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Build high-converting sales funnels, landing pages, and email sequences with an all-in-one German marketing platform.

## Description
Connect your **FunnelCockpit** account to any AI agent and take full control of your sales funnels and automated marketing workflows through natural conversation.

### What you can do

- **CRM & Contact Orchestration** — List and manage your entire customer database programmatically, retrieving detailed profile metadata and contact tags
- **Email Marketing Intelligence** — Programmatically retrieve your email lists and subscriber statuses to maintain a perfectly coordinated outreach strategy
- **Funnel & Page Monitoring** — Access your complete directory of active funnels and pages to oversee your conversion architecture in real-time
- **Webinar Intelligence Discovery** — Access real-time webinar registration metadata and attendee metrics directly through your agent for instant reporting
- **Operational Monitoring** — Verify account-level API connectivity and monitor orchestration volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **Private API Key** from your FunnelCockpit dashboard (Settings)
3. Start orchestrating your funnel growth from Claude, Cursor, or any MCP client

No more manual exporting of lead lists or missing webinar sign-ups. Your AI acts as your dedicated funnel coordinator and marketing architect.

### Who is this for?

- **Marketing Managers** — instantly retrieve funnel performance recaps and monitor email campaign results using natural language commands
- **Sales Leads** — verify individual CRM contact metadata and track webinar engagement without leaving your workspace
- **Developers** — integrate high-speed FunnelCockpit data into custom automation workflows through simple AI queries


## Available Tools
- **check_funnelcockpit_status**: Verify FunnelCockpit API connectivity
- **create_contact**: Create a CRM contact
- **get_account**: Get account info
- **get_contact**: Get contact details
- **get_funnel**: Get funnel details
- **list_campaigns**: List all campaigns
- **list_contacts**: List all CRM contacts
- **list_funnels**: List all funnels
- **list_pages**: List funnel pages
- **update_contact**: Pass a JSON string of field-value pairs to modify.

Update a CRM contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FunnelCockpit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active funnels in my FunnelCockpit account."

**🤖 AI Agent:**
> I've retrieved your funnels. You currently have 5 active profiles, including 'Main Sales Funnel' and 'Lead Magnet'. Would you like the detailed page metadata for any of them?

---

**👤 You:**
> "Check for new CRM contacts added today."

**🤖 AI Agent:**
> Contact directory orchestrated! I've identified 10 new profiles added today, including 'John Lead' and 'Acme Corp'. I've retrieved the technical tag metadata for your review. Shall I check their last funnel activity?

---

**👤 You:**
> "Show the registration count for the 'Upcoming Webinar'."

**🤖 AI Agent:**
> Webinar intelligence orchestrated! For 'Upcoming Webinar', I've identified 50 registered viewers. I've retrieved the registration source metadata for your review. Need help preparing the automated follow-up emails?


## Installation & Usage

To install and use the **FunnelCockpit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/funnelcockpit](https://vinkius.com/mcp/funnelcockpit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
