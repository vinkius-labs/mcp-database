# Better Stack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/better-stack-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Automate incident management via Better Stack — monitor uptime, manage incidents, and control on-call schedules securely from your AI agent.

## Description
Connect your **Better Stack (Better Uptime)** account to any AI agent and empower it to act as your Level 1 Site Reliability Engineer (SRE). Let your AI diagnose incidents, manage escalations, and audit monitoring configs securely via conversation.

### What you can do

- **Incident Response** — Rapidly list firing incidents, inspect technical downtime payloads, acknowledge alerts, and force resolve states inline
- **Uptime Monitors** — Fetch exact definitions of active HTTP endpoint pings, DNS probes, and latency constraints across your fleet
- **Cron Heartbeats** — Investigate passive tracking endpoints validating background workers and server limits
- **On-Call Management** — Expose active shifts and team schedules to determine explicitly who is getting paged in real-time
- **Status Pages** — Read configured public dashboards tracking your global infrastructure

### How it works

1. Subscribe to this server
2. Enter your Better Stack API Token
3. Empower Claude, Cursor, or your preferred agent to respond to alerts interactively

Stop switching context between your terminal and incident dashboards during critical outages.

### Who is this for?

- **DevOps & SREs** — audit on-call matrices safely, track firing pages, and orchestrate initial debugging workflows without leaving chat
- **Engineering Managers** — review recent downtime timelines and resolve dormant alerts quickly
- **Backend Developers** — rapidly debug failing cron heartbeats while simultaneously patching code


## Available Tools (10)
- **list_monitors**: List all monitors on Better Stack (Better Uptime)
- **get_monitor**: Get full details of a specific Better Stack monitor
- **list_incidents**: List all explicit incidents on Better Stack
- **get_incident**: Retrieve the native timeline payload of an explicit incident
- **acknowledge_incident**: Acknowledge an ongoing explicit incident halting paging
- **resolve_incident**: Force resolve a specific incident
- **list_heartbeats**: List all configured cron heartbeats securely
- **get_heartbeat**: Get explicit details of a passive heartbeat node
- **list_status_pages**: List all explicit Status Pages
- **list_on_call**: List exact On-Call routing calendars


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Better Stack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List any active unresolved incidents going on right now."

**🤖 AI Agent:**
> I found 1 active incident firing: ID #651239 (Critical API Down). It started 4 minutes ago and is currently escalating via phone call. Would you like me to acknowledge it locally?

---

**👤 You:**
> "Who is currently on-call for the main engineering shift?"

**🤖 AI Agent:**
> Looking at the calendar mapping, 'Core Backend Rotation' dictates John Doe is actively on call right now as Level 1, backed up formally by Jane Smith if escalation bypasses 10 minutes unconditionally.

---

**👤 You:**
> "Check the detailed root cause of passed Incident #8012."

**🤖 AI Agent:**
> Fetching incident #8012. The log dump points to a 502 Bad Gateway response received structurally from your Nginx server physically hosted in the EU region during the ping interval causing manual threshold failures.


## ❓ FAQ

**Q: Can my AI automatically acknowledge an incident so my phone stops ringing?**
Yes! Running the `acknowledge_incident` capability pushes a verified API command halting escalation cycles (like SMS and phone calls) natively while you debug.

**Q: Is it possible to see the exact HTTP response body or headers that caused a monitor to fail?**
Yes, pulling details via `get_incident` exposes the raw nested trace containing the root cause payloads and server errors Better Stack historically received when the check failed.

**Q: Can the agent create new monitors automatically?**
No. The integration focuses safely on observation, alerting resolution, and tracking currently. Creation endpoints represent mutation vectors decoupled to ensure you preserve billing and account structure intentionally.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/better-stack-1](https://vinkius.com/mcp/better-stack-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Better Stack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `better-stack-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Better Stack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "better-stack-1": {
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
