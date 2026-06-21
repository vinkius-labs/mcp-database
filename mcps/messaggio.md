# Messaggio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/messaggio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Send bulk SMS, Viber, and WhatsApp messages through a unified API with delivery tracking and campaign analytics.

## Description
### What you can do
Messaggio is a high-performance multi-channel messaging platform, and this MCP server brings its sophisticated routing and failover capabilities to your AI agents. Your assistant can now programmatically dispatch messages across SMS, Viber, and WhatsApp using a single unifed interface. The agent can define prioritized channel lists—for example, attempting delivery via WhatsApp first and automatically falling back to SMS if the message isn't read within a specified timeframe. Additionally, the assistant can monitor real-time delivery and read status, manage sender IDs for different projects, and send quick plain-text alerts. By integrating Messaggio with an AI agent, you transform your customer communication into a dynamic, context-aware engine that ensures your messages always reach their destination through the most effective channel.

### How it works
1. Log in to your Messaggio dashboard and locate your Project Login in the sender info section.
2. Connect your account using the provided secure setup instructions.
3. Your AI agent can now orchestrate complex messaging workflows, handling channel selection and status monitoring autonomously.

### Who is it for?
This integration is perfect for customer support teams needing reliable notification systems, marketing departments running multi-platform campaigns, and operations teams automating transactional alerts. By connecting Messaggio to an AI agent, you eliminate the complexity of managing separate APIs for each messaging app and allow your assistant to handle the failover logic and delivery optimization programmatically.


## Available Tools (12)
- **check_messaggio_status**: Verify connectivity
- **get_message_status**: Get message status
- **get_sender**: Get sender details
- **get_template**: Get template details
- **list_messages**: List messages
- **list_project_senders**: List project senders
- **list_projects**: List projects
- **list_senders**: List senders
- **list_templates**: List templates
- **send_bulk**: Send bulk messages
- **send_message**: Send a message
- **send_simple_sms**: Send SMS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Messaggio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a message to '79001234567' trying WhatsApp first, then SMS."

**🤖 AI Agent:**
> Configuring the multi-channel message with prioritized routing...

---

**👤 You:**
> "Check the status of my last 3 sent messages."

**🤖 AI Agent:**
> Retrieving the real-time delivery and read status for your messages...

---

**👤 You:**
> "List all verified sender IDs for the project 'PROJ-123'."

**🤖 AI Agent:**
> Fetching the list of senders associated with the specified project...


## ❓ FAQ

**Q: What is failover routing?**
It's the ability to automatically try alternative channels (like SMS) if the primary channel (like WhatsApp) fails or the message isn't read.

**Q: Can the agent check if a message was read?**
Yes, by using the get_messages_status tool, the agent can retrieve the 'read' status for supported channels like Viber and WhatsApp.

**Q: Does it support templates?**
Yes, you can configure WhatsApp and Viber templates in the Messaggio dashboard and have the agent trigger them via the send tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/messaggio](https://vinkius.com/mcp/messaggio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Messaggio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `messaggio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Messaggio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "messaggio": {
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
