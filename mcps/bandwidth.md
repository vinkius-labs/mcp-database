# Bandwidth MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bandwidth)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bandwidth-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bandwidth-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Automate telecom workflows via Bandwidth — send SMS/MMS, manage media, campaigns, and toll-free verification directly from any AI agent.

## Description
Connect your **Bandwidth** account to any AI agent and take full control of your cloud communications stack through natural conversation.

### O que você pode fazer

- **Messaging** — Instantly blast SMS and MMS (with rich media attachments) explicitly bypassing legacy SIP pipelines
- **10DLC Campaigns** — Validate 10DLC TCR profiling and approve messaging rules preventing carrier filtering
- **Toll-Free Verification** — Ping upstream toll-free approval headers checking compliance dynamically
- **Logs & Media** — Iterate over messaging histories, clear cached media payloads, and ensure API health routing

### Como funciona

1. Subscribe to this server
2. Enter your explicit Bandwidth Account ID, Username, and Password
3. Start dispatching text alerts, querying delivery footprints, or managing assets from Claude / Cursor

Scale unified communications reliably without building massive custom Webhook architectures. Your AI agent handles the underlying CPaaS native complexity.

### Para quem é?

- **Support Teams** — dispatch priority outage SMS blasts instantly out of Slack interfaces tracking message receipts
- **Marketing Operators** — audit 10DLC campaign health routing ensuring promotional texts never face upstream filtering blocks
- **DevOps Engineers** — ping the telecom backbone executing structural health tests before system scaling


## Available Tools
- **delete_media**: Delete a stored media asset
- **get_campaign**: Get details for a specific 10DLC campaign
- **get_toll_free**: List toll-free number verifications
- **get_health**: Ping Bandwidth API Health
- **list_applications**: List Messaging Applications
- **list_campaigns**: List 10DLC messaging campaigns
- **list_media**: List uploaded media files in Bandwidth storage
- **list_messages**: List sent or received messages log
- **send_mms**: Send an MMS message with media payload
- **send_sms**: Send an SMS message via Bandwidth API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bandwidth** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS from our main line +15551234567 to +18889990000 saying 'The server outage is fully resolved. Thank you.'"

**🤖 AI Agent:**
> I've successfully dispatched the SMS explicit payload to +18889990000. Bandwidth acknowledged the HTTP request and added it to the outbound carrier queue mapping your application ID.

---

**👤 You:**
> "List all uploaded media files on our account and delete any named 'old-marketing-promo.png'."

**🤖 AI Agent:**
> I identified 14 physical media blocks active within your Bandwidth hosting instance. The file named 'old-marketing-promo.png' was located and effectively removed via HTTP delete routing instantly freeing its storage consumption limits.

---

**👤 You:**
> "Ping the Bandwidth API Health check."

**🤖 AI Agent:**
> The structural check returned a 200 OK. The Bandwidth Messaging services are explicitly operating without upstream incidents or structural latency problems over current regions.


## Installation & Usage

To install and use the **Bandwidth** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bandwidth](https://vinkius.com/mcp/bandwidth)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
