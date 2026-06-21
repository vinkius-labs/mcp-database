# PagerDuty Incident Trigger MCP Server

This MCP does exactly one thing: it triggers incidents in PagerDuty. That's its only function, and nothing else. Incredible for giving your AI agents the power to wake up engineers.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pagerduty-incident-trigger)

## Overview
**Category:** industry-titans
**Tools Count:** 1

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


## Installation & Usage

To install and use the **PagerDuty Incident Trigger** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pagerduty-incident-trigger](https://vinkius.com/mcp/pagerduty-incident-trigger)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
