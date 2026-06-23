# Stannp MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stannp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate direct mail and physical letters via Stannp — manage letters, postcards, and campaigns directly from any AI agent.

## Description
Connect your **Stannp** account to any AI agent and simplify your direct mail marketing, physical letter delivery, and mailing list management through natural conversation.

### What you can do

- **Physical Mail Delivery** — Create and send single or bulk letters and postcards programmatically directly from your agent
- **Campaign Management** — Query all configured direct mail campaigns and retrieve detailed metadata and status
- **Recipient Control** — Query your database of contacts and mailing addresses to choose the right recipients for each piece
- **Account tracking** — Access your real-time account balance to manage your mailing spend
- **Live Monitoring** — Access a history of sent and drafted letters to stay on top of your physical outreach

### How it works

1. Subscribe to this server
2. Enter your Stannp API Key from your account settings
3. Start managing your direct mail from Claude, Cursor, or any MCP-compatible client


## Available Tools (11)
- **create_postcard**: Create and send a postcard
- **create_recipient**: Create a new mailing recipient
- **get_campaign**: Get details for a direct mail campaign
- **get_letter**: Get details for a specific letter
- **get_recipient**: Get details for a specific recipient
- **create_physical_letter**: Send a physical letter
- **get_account_balance**: Check account credit balance
- **list_direct_mail_campaigns**: List direct mail campaigns
- **list_letters**: List sent and drafted letters
- **list_postcards**: List sent and drafted postcards
- **list_mailing_recipients**: List mailing recipients


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stannp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my sent letters in Stannp."

**🤖 AI Agent:**
> I've retrieved your letters. You have 10 sent items, including 'Welcome Pack' and 'Invoice #123'.

---

**👤 You:**
> "Show me all direct mail campaigns with their delivery status and response rates."

**🤖 AI Agent:**
> 8 direct mail campaigns. Active (3): "Spring Promo Postcards" (2,340 sent, 2,280 delivered, 98 responses, 4.3% response rate, QR scans: 156). "VIP Thank You Letters" (120 sent, 118 delivered, personalized). "Re-engagement Mailer" (890 sent, in transit). Completed (4): avg 3.8% response rate. Draft (1): "Summer Sale Flyer" (ready for review). Total pieces mailed this month: 5,200. Total spend: £1,890. Average cost per piece: £0.36. Best performing: "Holiday Catalog" at 6.2% response.

---

**👤 You:**
> "Create and send a personalized postcard to our top 50 customers with a loyalty discount code."

**🤖 AI Agent:**
> Postcard campaign created: "VIP Loyalty Reward". Recipients: 50 top customers (by lifetime value). Personalization: first name, unique discount code per recipient (VIP-[NAME]-20). Design: A5 size, full-color front with product image, personalized back with message and QR code to redemption page. Print status: queued for next business day. Estimated delivery: 3-5 business days. Cost: £22.50 (£0.45/piece). Tracking: Royal Mail tracked. Redemption tracking: unique codes linked to CRM profiles.


## ❓ FAQ

**Q: Can I send a physical letter using my AI agent?**
Yes! Use the `create_physical_letter` action. Provide the recipient details and a template ID to trigger printing and mailing programmatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stannp](https://vinkius.com/mcp/stannp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stannp** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stannp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stannp** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stannp": {
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
