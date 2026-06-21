# Amazon EventBridge Bus MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amazon-eventbridge-bus)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Event-driven architecture for AI agents — scoped event dispatching strictly limited to one EventBus for zero-trust security.

## Description
Grant your AI agent **precise, scoped access** to a single Amazon EventBridge Bus. Unlike granting full AWS EventBridge permissions, this server adheres to the principle of least privilege, ensuring the agent can only dispatch `PutEvents` payloads to one specifically configured bus to trigger downstream orchestrations.

### What you can do

- **Put Events** — Dispatch custom JSON events specifying the `Source` and `DetailType` to trigger AWS Lambda functions, Step Functions, or third-party webhooks via EventBridge Rules.


## Available Tools (1)
- **put_events**: Send custom events to the Amazon EventBridge Bus


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amazon EventBridge Bus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Dispatch an event indicating that user registration was completed. Source: com.auth.service. Detail: {"userId": 999}."

**🤖 AI Agent:**
> Done! I've put the event into the EventBus. The downstream systems will now process it.

---

**👤 You:**
> "Send a 'FileUploaded' event from 'my.storage.bucket'."

**🤖 AI Agent:**
> Event successfully dispatched to EventBridge.

---

**👤 You:**
> "Trigger the daily audit pipeline by sending the 'AuditStarted' event."

**🤖 AI Agent:**
> I've successfully triggered the audit pipeline by putting the event in the configured bus.


## ❓ FAQ

**Q: Why limit the agent to a single bus?**
To enforce zero-trust security. An autonomous agent shouldn't be able to inject events into arbitrary event buses across your organization.

**Q: Can the agent receive events with this tool?**
No. EventBridge is designed for routing. To receive events back to an agent, you should route the EventBridge Rule to an SQS Queue and use the Amazon SQS Queue MCP.

**Q: What is the 'default' bus?**
Every AWS account has a 'default' event bus. If you haven't created a custom bus, you can simply type 'default' during configuration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amazon-eventbridge-bus](https://vinkius.com/mcp/amazon-eventbridge-bus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amazon EventBridge Bus** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `amazon-eventbridge-bus` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amazon EventBridge Bus** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amazon-eventbridge-bus": {
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
