# UK Postbox MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uk-postbox)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your virtual mailbox via UK Postbox u2014 scan letters, forward mail, send correspondence, and track parcels from your AI agent.

## Description
Connect your **UK Postbox** account to any AI agent and manage your virtual mailbox, scan letters, forward parcels, and send physical mail through natural conversation.

### What you can do

- **Mail Management** u2014 List, view, and scan all incoming letters and envelopes in your virtual postbox
- **Mail Forwarding** u2014 Forward physical mail to any saved address with full tracking
- **Letter Sending** u2014 Compose and send physical letters via Royal Mail directly from your AI agent
- **Parcel Tracking** u2014 View and manage all parcels with dimensions, weight, and storage status
- **Address Book** u2014 Manage your saved forwarding addresses for quick mail routing

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from the UK Postbox integrations page
3. Start managing your virtual mail from Claude, Cursor, or any MCP client

### Who is this for?

- **Remote Workers** u2014 manage your UK mail from anywhere in the world
- **Business Owners** u2014 automate mail scanning and forwarding for multiple locations
- **Expats & Travelers** u2014 stay on top of important correspondence without a physical presence


## Available Tools (10)
- **check_ukpostbox_status**: Verify UK Postbox API connectivity
- **forward_mail**: Forward mail
- **get_mail_item**: Get mail item details
- **get_mail_scan**: Get mail scan
- **get_parcel**: Get parcel details
- **list_addresses**: List forwarding addresses
- **list_mail_items**: List all mail items
- **list_parcels**: List all parcels
- **request_scan**: Request a mail scan
- **send_letter**: Provide recipient name, full address, and letter content.

Send a letter


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UK Postbox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all unread mail in my virtual postbox."

**🤖 AI Agent:**
> You have 6 unread items: 3 letters, 2 parcels, 1 large envelope. The most recent letter is from HMRC, received today. Would you like to scan it?

---

**👤 You:**
> "Scan the letter from HMRC and forward it to my home address."

**🤖 AI Agent:**
> Scan requested for the HMRC letter — it will be ready within 2 hours. I've also queued it for forwarding to your home address (London, SW1A 1AA). You'll receive tracking once posted.

---

**👤 You:**
> "Send a letter to John Smith at 10 Downing Street."

**🤖 AI Agent:**
> Letter queued for printing and posting. Recipient: John Smith, 10 Downing Street, London, SW1A 2AA. Estimated delivery: 1-2 business days via Royal Mail. Would you like a tracking reference?


## ❓ FAQ

**Q: Can I scan my mail remotely via AI?**
Yes. Use `request_scan` with the mail item ID to open and digitize a letter. Then use `get_mail_scan` to view the scanned document.

**Q: How do I forward mail to another address?**
Use `forward_mail` with the mail item ID and a forwarding address ID from your saved addresses. Check `list_addresses` for available destinations.

**Q: Can I send physical letters from my agent?**
Absolutely. Use `send_letter` with the recipient name, postal address, and letter content. The letter is printed and posted via Royal Mail.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uk-postbox](https://vinkius.com/mcp/uk-postbox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UK Postbox** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `uk-postbox` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UK Postbox** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "uk-postbox": {
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
