# Bandwidth MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bandwidth)
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


## ❓ FAQ

**Q: Can my AI agent check if my 10DLC campaign is cleared for high-volume SMS?**
Yes. Ask the agent to list your 10DLC campaigns or check a specific campaign ID. It natively surfaces throughput limits (like TPS bounds) set by TCR preventing you from getting blocked by aggressive mobile carriers.

**Q: How do I troubleshoot SMS delivery failures using the agent?**
You can tell the agent to 'List messages filtered by phone number +1XXXXXXXXXX'. The tool natively reaches Bandwidth's logs and pulls exactly what operational state the message failed in, bypassing complex raw log exports.

**Q: Does the system support sending localized multimedia messages (MMS) directly?**
Yes. Provide the agent with the from address, the to address, the text block, and a direct URL to a hosted JPEG/PNG image. The agent explicitly commands the send_mms tool injecting image packets into the phone line seamlessly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bandwidth](https://vinkius.com/mcp/bandwidth)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bandwidth** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bandwidth` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bandwidth** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bandwidth": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
