# Flowcode MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flowcode)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/flowcode-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/flowcode-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage dynamic QR codes, track scan analytics, and oversee Flowpages via AI agents with Flowcode.

## Description
Connect your **Flowcode** account to any AI agent and automate your offline-to-online marketing through the Model Context Protocol (MCP). Flowcode is the leading platform for dynamic QR codes and conversion-optimized landing pages (Flowpages). Now, you can create new codes, monitor scan performance, and retrieve deep audience analytics directly through natural conversation.

### What you can do

- **Dynamic QR Management** — List all your Flowcodes, fetch detailed metadata, and create new dynamic codes with instant redirect capabilities.
- **Scan Analytics** — Monitor real-time scan performance, conversion rates, and detailed scan activity logs to optimize your campaigns.
- **Flowpage Oversight** — Retrieve real-time event data for your landing pages and access CRM contact information submitted via Flowpage forms.
- **Audience Insights** — Fetch aggregate demographic and geographic analytics to understand where and how your audience is engaging.
- **Asset Organization** — List campaigns and asset folders to maintain a clear structure across your marketing projects.
- **Image Generation** — Retrieve specific Flowcode image data or download links directly from the agent.
- **Custom Conversions** — Track conversion rates from scan to visit to ensure your marketing funnel is performing optimally.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Flowcode API Key (found in your Flowcode Developer Portal)
3. Start managing your dynamic QR codes and analytics from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing Managers** — quickly create a new QR code for a print campaign or check scan stats before a meeting.
- **Brand Operations** — get a real-time overview of geographic engagement across all active Flowcodes through simple AI commands.
- **Sales Teams** — automate the retrieval of lead contact info submitted through offline QR code interactions.


## Available Tools
- **create_flowcode**: Create a dynamic QR code
- **get_flowpage_contacts**: Get CRM contacts
- **get_audience_summary**: Get audience demographics
- **get_flowcode_image**: Generate QR code image
- **get_flowcode**: Get Flowcode details
- **get_flowpage_analytics**: Get landing page events
- **get_geographic_analytics**: Get scan locations
- **get_recent_scans**: List scan activity log
- **list_campaigns**: List marketing campaigns
- **list_conversion_rates**: Get funnel analytics
- **list_flowcodes**: List all Flowcodes
- **list_folders**: List asset folders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flowcode** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my 10 most recent Flowcodes and their scan counts."

**🤖 AI Agent:**
> Fetching Flowcodes... I found your 10 most recent dynamic QR codes, including 'Fall Campaign' (1,250 scans) and 'Product Demo' (450 scans). Would you like to see the geo-analytics for any of these?

---

**👤 You:**
> "Create a new Flowcode named 'Store Launch' redirecting to 'https://vinkius.com'."

**🤖 AI Agent:**
> Flowcode created! I've generated a new dynamic QR code named 'Store Launch' pointing to vinkius.com. The code ID is 'code_123'. I can provide the image download link whenever you're ready.

---

**👤 You:**
> "Show me the audience demographic summary for my account."

**🤖 AI Agent:**
> Retrieving audience data... Your engagement is primarily coming from users aged 25-34 (45%) using mobile devices. The top scan locations are New York and London. Would you like a more detailed breakdown?


## Installation & Usage

To install and use the **Flowcode** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flowcode](https://vinkius.com/mcp/flowcode)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
