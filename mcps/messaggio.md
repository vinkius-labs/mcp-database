# Messaggio MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/messaggio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/messaggio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/messaggio-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Messaggio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/messaggio](https://vinkius.com/mcp/messaggio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
