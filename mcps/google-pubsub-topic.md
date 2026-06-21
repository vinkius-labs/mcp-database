# Google Pub/Sub Topic MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-pubsub-topic)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

This MCP does exactly one thing: it publishes messages to a single Google Pub/Sub Topic. That's its only function, and nothing else. Incredible for giving your AI the power to trigger cloud events.

## Description
This server strips away dangerous global GCP permissions. It gives your AI agent one surgical superpower: **the ability to publish messages and trigger events on one specific Pub/Sub Topic.**

By strictly scoping access, your AI can safely fan out notifications, trigger downstream workers, and emit system alerts without ever compromising the rest of your messaging infrastructure.

### The Superpowers

- **Absolute Containment:** The agent is locked to a single topic. It cannot publish to other topics or alter topic configurations.
- **Native Pub/Sub Integration:** Send payloads with advanced message attributes.
- **Plug & Play Event Trigger:** Instantly gives your agent the ability to act as an event producer in your distributed system architecture.


## Available Tools (1)
- **pubsub_publish_message**: Publish a message to the configured Google Cloud Pub/Sub Topic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Pub/Sub Topic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Publish an event indicating that the user sign-up was verified."

**🤖 AI Agent:**
> Done! I've published the message to the topic. The generated Message ID is '3910398201'.

---

**👤 You:**
> "Send the invoice payload to the topic with the attribute 'type=invoice_ready'."

**🤖 AI Agent:**
> The payload was successfully published. The attribute 'type: invoice_ready' was attached for downstream filtering.

---

**👤 You:**
> "Trigger the background data export via Pub/Sub."

**🤖 AI Agent:**
> Message sent. The workers subscribed to the topic will now begin the background export process.


## ❓ FAQ

**Q: Why limit the agent to a single Pub/Sub Topic?**
To enforce zero-trust architecture. An autonomous AI agent should not have the ability to publish events to arbitrary critical infrastructure topics (e.g., billing alerts or user deletion events).

**Q: Do I need to base64-encode my messages manually?**
No. Provide plain text or JSON strings directly to the tool. The engine will automatically convert your payload to base64 as required by the Google Cloud Pub/Sub REST API.

**Q: Can the agent receive messages with this tool?**
No. This tool only has `publish_message` capabilities to enforce unidirectional isolation. If the agent needs to receive messages, it must use the Google Pub/Sub Subscription MCP.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-pubsub-topic](https://vinkius.com/mcp/google-pubsub-topic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Pub/Sub Topic** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `google-pubsub-topic` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Pub/Sub Topic** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-pubsub-topic": {
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
