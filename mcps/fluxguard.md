# Fluxguard MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fluxguard)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fluxguard-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fluxguard-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Monitor website changes, track visual differences, and receive alerts via AI agents with Fluxguard.

## Description
Connect your **Fluxguard** account to any AI agent to automate website change monitoring and regression testing. Fluxguard provides a comprehensive platform for detecting text, HTML, and visual changes across your monitored pages. This MCP server allows you to manage your monitoring setup and retrieve change alerts directly through natural conversation.

### What you can do

- **Page Monitoring** — Add new URLs for monitoring and organize them into categories.
- **Change Detection** — Retrieve a list of all detected changes and fetch specific details for each change.
- **Manual Crawls** — Manually initiate immediate crawls for your monitored sites.
- **Alert Management** — Access all generated alerts and acknowledge them directly through the agent.
- **Snapshots** — List and retrieve historical snapshots captured for your monitored pages.
- **AI Summaries** — Detected changes can be summarized to understand the significance of every update.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Fluxguard API Key (obtained from your Organization Settings)
3. Start managing your website monitoring directly from your AI agent


## Available Tools
- **acknowledge_alert**: Mark alert as reviewed
- **add_page**: Add URL for monitoring
- **create_category**: Create a new category
- **get_account**: Get organization attributes
- **get_change**: Get change details
- **get_site**: Get site details
- **initiate_crawl**: Manually trigger a crawl
- **list_alerts**: List monitoring alerts
- **list_categories**: List monitoring categories
- **list_changes**: List detected changes
- **list_sites**: List monitored sites
- **list_snapshots**: List site snapshots


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fluxguard** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add the URL 'https://example.com' to my monitoring list."

**🤖 AI Agent:**
> Adding page... 'https://example.com' has been successfully added to your monitoring list.

---

**👤 You:**
> "Show me the most recent changes detected across all sites."

**🤖 AI Agent:**
> Retrieving changes... I found 3 recent changes across your monitored pages.

---

**👤 You:**
> "Initiate an immediate crawl for site ID 'site_123'."

**🤖 AI Agent:**
> Crawl initiated! I've started an immediate crawl for site ID 'site_123'.


## Installation & Usage

To install and use the **Fluxguard** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fluxguard](https://vinkius.com/mcp/fluxguard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
