# Telnyx Fax MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/telnyx-fax)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Send, receive, and manage faxes via Telnyx u2014 transmit documents, track delivery, and manage fax numbers from your AI agent.

## Description
Connect your **Telnyx** account to any AI agent and send, receive, and manage faxes through natural conversation.

### What you can do

- **Send Faxes** u2014 Transmit PDF and TIFF documents to any fax number worldwide with delivery tracking
- **Fax Management** u2014 List all sent and received faxes, check delivery status, and cancel queued transmissions
- **Phone Numbers** u2014 View and manage all fax-enabled phone numbers in your Telnyx account
- **Fax Applications** u2014 Browse and configure your fax application settings including webhook URLs
- **Media Library** u2014 Access all uploaded documents available for faxing

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from the Telnyx Mission Control portal
3. Start sending and managing faxes from Claude, Cursor, or any MCP client

### Who is this for?

- **Healthcare & Legal Teams** u2014 send compliant documents via secure fax directly from your AI workflow
- **Operations Teams** u2014 automate high-volume fax delivery with real-time status tracking
- **Developers** u2014 integrate fax capabilities into automated pipelines via simple AI queries


## Available Tools (10)
- **check_telnyx_status**: Verify Telnyx API connectivity
- **get_fax_application**: Get fax application details
- **get_fax**: Get fax details
- **get_fax_number**: Get phone number details
- **list_fax_applications**: List fax applications
- **list_faxes**: List all faxes
- **list_media**: List media files
- **list_fax_numbers**: List fax-enabled numbers
- **send_fax**: Requires connection ID (from), recipient number, and media URL.

Send a fax
- **cancel_fax**: Cancel a fax


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Telnyx Fax** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a fax of invoice.pdf to +1-555-0199."

**🤖 AI Agent:**
> Fax submitted to +15550199. Fax ID: FAX-8291. Transmission in progress — 3 pages detected. Would you like me to check the delivery status in a few minutes?

---

**👤 You:**
> "List all faxes sent today."

**🤖 AI Agent:**
> 5 faxes sent today. 4 delivered successfully, 1 still in progress (FAX-8291 to +15550199). Total pages transmitted: 14. Would you like details on any specific fax?

---

**👤 You:**
> "Show my fax-enabled phone numbers."

**🤖 AI Agent:**
> You have 3 fax-enabled numbers: +1-555-0100 (US), +44-20-7946-0958 (UK), and +1-555-0200 (US toll-free). All active and ready to send/receive faxes.


## ❓ FAQ

**Q: How do I send a fax via AI?**
Use the `send_fax` tool with your connection ID, recipient phone number (E.164 format), and a URL to the PDF or TIFF document.

**Q: Can I check the status of a sent fax?**
Yes. Use `get_fax` with the fax ID to see delivery status, page count, duration, and any error details.

**Q: How do I see my fax-enabled phone numbers?**
Use `list_fax_numbers` to retrieve all phone numbers in your Telnyx account that have fax capability enabled.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/telnyx-fax](https://vinkius.com/mcp/telnyx-fax)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Telnyx Fax** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `telnyx-fax` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Telnyx Fax** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "telnyx-fax": {
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
