# WA Smart Business MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wa-smart-business-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Scale your WhatsApp business communication with chatbots, bulk messaging, and team inbox features for growing companies.

## Description
Connect your **WA Smart Business** account to any AI agent and take full control of your WhatsApp marketing automation and customer service workflows through natural conversation.

### What you can do

- **WhatsApp Orchestration** — Programmatically send high-fidelity text and media messages (Images, PDF, Video) to customers via the official WhatsApp Business Platform
- **Contact Intelligence** — List and manage your high-fidelity customer database, retrieving detailed profile metadata and custom dynamic field updates
- **Team & Agent Architecture** — Access your complete directory of support agents and coordinate assignments to maintain a perfectly coordinated response team
- **Engagement Monitoring** — Access real-time message delivery statuses and track customer interaction metrics directly through your agent for instant reporting
- **Operational Monitoring** — Verify account-level API connectivity and monitor messaging volume directly through your agent for perfectly coordinated scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your WA Smart Business dashboard (Settings > API)
3. Start orchestrating your WhatsApp communications from Claude, Cursor, or any MCP client

No more manual toggling between WhatsApp tabs or missing critical customer replies. Your AI acts as your dedicated communications coordinator and messaging architect.

### Who is this for?

- **Marketing Managers** — instantly trigger WhatsApp campaigns and monitor delivery rates using natural language commands
- **Support Leads** — coordinate agent assignments and verify response quality without leaving your workspace
- **Developers** — integrate high-speed WhatsApp Cloud API data into custom internal tools through simple AI queries


## Available Tools (13)
- **check_wasmart_status**: Verify connectivity
- **create_customer**: Create a customer
- **get_agent**: Get agent details
- **get_customer**: Get customer details
- **list_agents**: List agents
- **list_campaigns**: List campaigns
- **list_customers**: List customers
- **list_messages**: List messages
- **list_templates**: List templates
- **search_customers**: Search customers
- **send_media**: Send media
- **send_message**: Send a message
- **send_template**: Send a template


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WA Smart Business** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active customers in my WA Smart Business account."

**🤖 AI Agent:**
> I've retrieved your customer directory. You currently have 300 active profiles, including 'Sarah Manager' and 'Mike Client'. Would you like the detailed high-fidelity metadata for any of them?

---

**👤 You:**
> "Send a WhatsApp image to '+15550123': 'https://example.com/promo.png'."

**🤖 AI Agent:**
> WhatsApp orchestrated! I've successfully sent the high-fidelity promotional image to +15550123. The message is now active in your engagement history. Need help checking the delivery status?

---

**👤 You:**
> "Check which support agents are currently assigned to 'Mike Client'."

**🤖 AI Agent:**
> Agent architecture orchestrated! Mike Client is currently assigned to 'Agent_789' (John Doe). I've retrieved the high-fidelity assignment metadata and last interaction duration for your review. Shall I reassign this customer?


## ❓ FAQ

**Q: How do I find my WA Smart Business API Key?**
Log in to your account, navigate to **Settings** > **API**, and copy your unique Access Token or API Key from the credentials section.

**Q: Can I send PDFs or Images via AI?**
Yes! The `send_whatsapp_media` tool allows your agent to send high-fidelity files by providing the recipient's number and the media URL.

**Q: How do I list my support agents?**
Use the `list_whatsapp_agents` tool to retrieve your complete high-fidelity directory along with the current assignments for all team members.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wa-smart-business-alternative](https://vinkius.com/mcp/wa-smart-business-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WA Smart Business** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wa-smart-business-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WA Smart Business** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wa-smart-business-alternative": {
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
