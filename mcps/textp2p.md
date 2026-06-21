# TextP2P MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/textp2p)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/textp2p-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/textp2p-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Send peer-to-peer text messages at scale for political campaigns, nonprofits, and organizations that need personal outreach.

## Description
Connect your **TextP2P** marketing account to any AI agent and simplify how you manage your bulk SMS campaigns, ringless voicemails (RVM), and contact lists through natural conversation.

### What you can do

- **Multi-channel Messaging** — Send individual or mass SMS and MMS messages with full media support.
- **Ringless Voicemail (RVM)** — Drop recorded voicemails directly to mobile numbers without making the phone ring.
- **Contact Management** — Add new recipients and manage your marketing lists to keep your outreach organized.
- **List Oversight** — List and query all your mailing groups and segments to target the right audience.
- **Account Visibility** — Retrieve your current credit balance for SMS, MMS, and RVM to monitor your budget.
- **Operational Monitoring** — Track your messaging activities and credit usage directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your TextP2P API URL, Username, and API Secret
3. Start managing your bulk messaging campaigns from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing & Sales Teams** — quickly execute mass SMS campaigns and check credit balances via simple AI commands.
- **Operations Managers** — automate the creation of contact lists and monitor RVM broadcasts directly from the workspace.
- **Small Business Owners** — maintain personal contact with customers through professional text and voice automation via the AI assistant.


## Available Tools
- **add_textp2p_contact**: Add a new contact
- **get_textp2p_balance**: Get account credit balance
- **list_textp2p_lists**: List all contact lists
- **send_textp2p_mms**: Send an MMS message
- **send_textp2p_rvm**: Send a Ringless Voicemail (RVM)
- **send_textp2p_sms**: Send an SMS message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TextP2P** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a bulk SMS to '555-0199, 555-0188' saying: 'Flash sale ends in 2 hours!'."

**🤖 AI Agent:**
> SMS campaign initiated! I've sent the message to both recipients. I'll let you know if you need to check your remaining credit balance after this broadcast.

---

**👤 You:**
> "Drop a ringless voicemail to +15550177 using audio URL 'https://vinkius.com/vmail.mp3'."

**🤖 AI Agent:**
> RVM request sent! I've triggered the ringless voicemail drop to +15550177 with your audio file. It will be delivered directly to the recipient's inbox without ringing.

---

**👤 You:**
> "Check my current credit balance for SMS and RVM."

**🤖 AI Agent:**
> Fetching balance... You currently have 1,200 SMS credits and 450 RVM credits available. You have plenty of budget for your upcoming marketing campaigns.


## Installation & Usage

To install and use the **TextP2P** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/textp2p](https://vinkius.com/mcp/textp2p)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
