# PagerDuty Incident Trigger MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pagerduty-incident-trigger)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pagerduty-incident-trigger-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pagerduty-incident-trigger-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

This MCP does exactly one thing: it triggers incidents in PagerDuty. That's its only function, and nothing else. Incredible for giving your AI agents the power to wake up engineers.

## Description
We refused to build a bloated incident management integration that attempts to manage on-call schedules, resolve tickets, or query PagerDuty REST APIs. Instead, this MCP server provides a surgical, zero-trust bridge: **just triggering incidents via the Events API V2.**

Your AI agent gains the immediate, zero-friction ability to evaluate anomalies and instantly escalate critical issues directly to the on-call engineer's phone.

### The Superpowers

- **Instant Escalation:** Give your agent the authority to declare a 'Critical' state. The agent provides a summary, source, and severity, and PagerDuty handles the paging.
- **Zero-Bloat Integration:** No massive SDKs or complex OAuth flows. Just a single Integration Key (Routing Key) is required to push events.
- **Absolute Containment:** Because this uses the one-way Events API V2, the agent cannot read your incident history, cannot modify on-call schedules, and cannot snoop on resolving engineers. It is the purest, safest way to give your AI paging superpowers.


## Available Tools
- **trigger_pagerduty_incident**: Provide a clear summary, the source of the issue, and an optional severity level ("critical", "error", "warning", "info"). Defaults to critical.

Trigger an incident in PagerDuty using the Events API V2


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PagerDuty Incident Trigger** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Trigger a critical PagerDuty incident for the payment-gateway saying transactions are failing."

**🤖 AI Agent:**
> I've successfully triggered the critical incident in PagerDuty.


## Installation & Usage

To install and use the **PagerDuty Incident Trigger** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pagerduty-incident-trigger](https://vinkius.com/mcp/pagerduty-incident-trigger)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
