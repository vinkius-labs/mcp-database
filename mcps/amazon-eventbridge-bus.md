# Amazon EventBridge Bus MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amazon-eventbridge-bus)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/amazon-eventbridge-bus-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/amazon-eventbridge-bus-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Event-driven architecture for AI agents — scoped event dispatching strictly limited to one EventBus for zero-trust security.

## Description
Grant your AI agent **precise, scoped access** to a single Amazon EventBridge Bus. Unlike granting full AWS EventBridge permissions, this server adheres to the principle of least privilege, ensuring the agent can only dispatch `PutEvents` payloads to one specifically configured bus to trigger downstream orchestrations.

### What you can do

- **Put Events** — Dispatch custom JSON events specifying the `Source` and `DetailType` to trigger AWS Lambda functions, Step Functions, or third-party webhooks via EventBridge Rules.


## Available Tools
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


## Installation & Usage

To install and use the **Amazon EventBridge Bus** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amazon-eventbridge-bus](https://vinkius.com/mcp/amazon-eventbridge-bus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
