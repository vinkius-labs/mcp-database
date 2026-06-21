# Microsoft Teams Webhook Notifier MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/microsoft-teams-webhook-notifier)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/microsoft-teams-webhook-notifier-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/microsoft-teams-webhook-notifier-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

This MCP does exactly one thing: it sends messages to your Microsoft Teams channels. That's its only function, and nothing else. Incredible for giving your AI agents a voice.

## Description
We refused to build a bloated Microsoft 365 integration that demands terrifying `ChannelMessage.Send` permissions across your entire corporate tenant via Microsoft Graph. Instead, this MCP server provides a surgical, zero-trust bridge: **a single Incoming Webhook URL.**

Your AI agent gains the immediate, zero-friction ability to drop critical alerts, deployment statuses, and rich engineering reports straight into the designated Teams channel without compromising your organization's Azure AD security.

### The Superpowers

- **Zero-Bloat Deployment:** No heavy Enterprise Apps to approve, no Graph API tokens to rotate. If you can generate a webhook, your AI can speak.
- **Native Adaptive Cards Mastery:** The agent isn't limited to boring plain text. It can programmatically generate rich Adaptive Cards or MessageCards—complete with actionable buttons, data tables, and structured telemetry.
- **Absolute Containment:** Because it's just a webhook, the agent cannot read your corporate emails, cannot snoop on other Teams channels, and cannot cause chaos. It is the purest, safest way to give your AI a megaphone in the enterprise world.


## Available Tools
- **send_teams_message**: Provide the fallback text in the "text" parameter. Optionally, provide a rich UI element via the "cardJson" string.

Send a notification or message to a Microsoft Teams channel via Webhook


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Microsoft Teams Webhook Notifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Notify Teams that the deployment is complete."

**🤖 AI Agent:**
> I've sent the message 'The deployment is complete.' to the Teams channel.

---

**👤 You:**
> "Send a rich alert to Teams using a MessageCard format to report a bug."

**🤖 AI Agent:**
> The rich MessageCard alert detailing the bug has been successfully posted to Teams.


## Installation & Usage

To install and use the **Microsoft Teams Webhook Notifier** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/microsoft-teams-webhook-notifier](https://vinkius.com/mcp/microsoft-teams-webhook-notifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
