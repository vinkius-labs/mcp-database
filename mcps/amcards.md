# AMcards MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amcards)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Send personalized greeting cards and handwritten notes to clients and prospects that feel genuinely personal at scale.

## Description
Connect your **AMcards** account to any AI agent and take full control of your automated physical relationship management and high-fidelity gifting workflows through natural conversation.

### What you can do

- **Physical Card Orchestration** — Programmatically dispatch personalized greeting cards with custom messages directly to any address without leaving your chat
- **Drip Campaign Intelligence** — Enroll leads or clients into automated card-sending sequences to maintain a perfectly coordinated relationship lifecycle in real-time
- **Template Management Architecture** — Access and monitor your complete library of card templates to ensure your high-fidelity brand voice is consistently applied
- **Delivery & History Tracking** — Retrieve detailed historical records of sent cards and monitor their delivery status directly through your agent for instant reporting
- **System Monitoring** — Access account-level profile metadata and verify API connectivity directly through your agent to maintain high-fidelity operations

### How it works

1. Subscribe to this server
2. Retrieve your **Access Token** from your AMcards dashboard (Settings > API)
3. Start sending real mail and gifts from Claude, Cursor, or any MCP client

No more manual logging into mailing portals to send thank-you notes. Your AI acts as your dedicated relationship engineer and physical mail coordinator.

### Who is this for?

- **Sales Professionals** — instantly send personalized 'Thank You' cards after a meeting using natural language commands
- **Customer Success Teams** — automate the dispatch of appreciation gifts and follow-ups without leaving your workspace
- **Real Estate Agents** — orchestrate long-term high-fidelity drip campaigns to maintain top-of-mind awareness through simple AI queries


## Available Tools
- **check_api_health**: com service API.

Verify AMcards API connectivity
- **get_card_sending_history**: Retrieve card sending history
- **list_drip_campaigns**: List automated drip campaigns
- **list_card_templates**: List greeting card templates
- **list_configured_webhooks**: List active webhooks
- **send_greeting_card**: Send a personalized greeting card
- **trigger_drip_campaign**: Start a drip campaign for a user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AMcards** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my physical card templates in AMcards."

**🤖 AI Agent:**
> I've retrieved your card library. You currently have 5 active templates, including 'Modern Thank You' (ID: 92) and 'New Client Welcome'. Which one should we use for your next mailing?

---

**👤 You:**
> "Send a 'Welcome' card (ID: '92') to 'John Smith' at '123 Main St, New York, NY 10001'."

**🤖 AI Agent:**
> Mailing orchestrated! I've successfully triggered the shipment of the Welcome card to John Smith. The order is now being processed for high-fidelity physical delivery. Need a copy of the message logs?

---

**👤 You:**
> "Show my recent card sending history and statuses."

**🤖 AI Agent:**
> Accessing shipment logs... Your last 5 shipments include 3 'Delivered' cards and 2 'In Transit'. The most recent was a gift bundle to @user1. Would you like the high-fidelity tracking numbers?


## ❓ FAQ

**Q: How do I find my AMcards Access Token?**
Log in to your account, navigate to **Settings** > **API**, and generate a new Access Token for your integration.

**Q: Can I include a gift with the card?**
Yes! If your chosen template ID includes a gift (like brownies), the system will automatically process the high-fidelity gifting workflow.

**Q: How do I check if a card was delivered?**
Use the `get_card_sending_history` tool to retrieve the high-fidelity status log of all your previous card shipments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amcards](https://vinkius.com/mcp/amcards)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AMcards** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `amcards` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AMcards** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amcards": {
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
