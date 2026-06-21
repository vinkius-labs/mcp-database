# PagerDuty Incident Trigger MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pagerduty-incident-trigger)
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


## ❓ FAQ

**Q: Can the agent resolve PagerDuty incidents with this?**
No. This MCP exclusively uses the 'trigger' event action. It cannot resolve or acknowledge incidents. Its sole purpose is to wake up human operators when it detects a critical anomaly.

**Q: How do I get a PagerDuty Integration Key?**
In PagerDuty, go to Services > Service Directory. Select your service, go to the Integrations tab, and add a new 'Events API V2' integration. Copy the resulting Integration Key.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pagerduty-incident-trigger](https://vinkius.com/mcp/pagerduty-incident-trigger)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PagerDuty Incident Trigger** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pagerduty-incident-trigger` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PagerDuty Incident Trigger** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pagerduty-incident-trigger": {
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
