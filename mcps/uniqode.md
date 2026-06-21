# Uniqode MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uniqode)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/uniqode-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/uniqode-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Create trackable QR codes with custom branding, dynamic content updates, and scan analytics for marketing and operations.

## Description
Connect your **Uniqode (formerly Beaconstac)** account to any AI agent and simplify how you create, manage, and analyze your QR code campaigns through natural conversation.

### What you can do

- **QR Code Generation** — Create dynamic or static QR codes for websites, vCards, or social media with full branding control.
- **Scan Analytics** — Retrieve detailed scan metrics by time, location (country/city), and device type to measure campaign performance.
- **Dynamic Updates** — Update the destination URL of your dynamic QR codes instantly without changing the physical code.
- **Organization Oversight** — List and manage QR codes across different organizations, folders, and campaigns.
- **Lifecycle Management** — Tag, categorize, and delete QR codes to keep your marketing dashboard organized.
- **Account Visibility** — Fetch account details and organization structures directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Uniqode API Key (found in your account settings)
3. Start managing your QR code ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing Managers** — quickly update campaign destinations and check scan analytics via simple AI queries.
- **Operations Teams** — automate the creation of vCard QR codes for staff and manage organizational folders.
- **Business Owners** — monitor customer engagement and physical-to-digital attribution directly from the workspace.


## Available Tools
- **create_qrcode**: qr_type: 1 for Website, 2 for vCard, etc.

Create a new QR code
- **delete_qrcode**: Delete a QR code
- **get_account_info**: Get account details
- **get_analytics_location**: Get scan analytics by location
- **get_analytics_time**: Get scan analytics by time
- **get_qrcode**: Get QR code details
- **list_campaigns**: List campaigns
- **list_folders**: List folders
- **list_organizations**: List organizations
- **list_qrcodes**: List all QR codes
- **list_tags**: List tags
- **update_qrcode**: Update an existing QR code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Uniqode** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my QR codes."

**🤖 AI Agent:**
> I've retrieved your QR codes. You have 12 active codes including 'Winter Sale 2024', 'Support vCard', and 'Menu - Main Branch'. Which one would you like scan analytics for?

---

**👤 You:**
> "Show me scan analytics for the 'Winter Sale' QR code by location."

**🤖 AI Agent:**
> Fetching geographic data... The 'Winter Sale' code has been scanned 450 times. Top locations include United States (210 scans), United Kingdom (105), and Canada (85). Shall I break it down by city?

---

**👤 You:**
> "Change the destination of QR code '10293' to 'https://vinkius.com/new-promo'."

**🤖 AI Agent:**
> Update successful! QR code 10293 is now redirecting to 'https://vinkius.com/new-promo'. The physical QR code remains valid and will instantly lead users to the new page.


## Installation & Usage

To install and use the **Uniqode** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uniqode](https://vinkius.com/mcp/uniqode)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
