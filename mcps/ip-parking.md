# IP Parking MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ip-parking)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage PARCS operations: sites, tariffs, gates, and ANPR events via IP Parking API.

## Description
Connect **IP Parking** to any AI agent and streamline your Parking Access and Revenue Control System (PARCS) — manage occupancy, update tariffs, control gates, and audit transactions through natural conversation.

### What you can do
- **Site Management** — Monitor real-time occupancy and revenue across all locations
- **Tariff Configuration** — View and modify hourly rates and pricing rules instantly
- **Gate Control** — Remotely open/close barriers for assistance or maintenance
- **Hardware Monitoring** — Check health of ANPR cameras, ticket dispensers, and gates
- **Transaction Auditing** — Review exit logs and revenue collection
- **ANPR Integration** — Register or simulate license plate recognition events

### How it works
1. Subscribe to this server
2. Enter your IP Parking API Key and Base URL
3. Start managing your parking infrastructure from Claude, Cursor, or any MCP-compatible client

IP Parking is a Dutch developer of web-based PARCS hardware and software, enabling barrierless and smart parking solutions.

### Who is this for?
- **Parking Operators** — Adjust tariffs and check occupancy without logging into the central management system
- **Support Teams** — Remotely open stuck gates and verify camera status via voice or text commands
- **Revenue Auditors** — Quickly query transaction logs and verify daily income


## Available Tools
- **register_anpr**: Used for testing or manual override of entry/exit.

Simulate or register an ANPR (License Plate Recognition) event
- **control_gate**: Remotely open or close a barrier gate.. Actions: default
- **list_hardware**: List hardware status (ANPR cameras, ticket machines, gates)
- **get_site_status**: Get real-time occupancy and revenue status for a site
- **list_sites**: List all managed parking sites
- **get_system_health**: Get overall system health and connectivity status
- **list_tariffs**: List active tariff rules
- **get_ticket_details**: Get details of a specific parking ticket/session
- **list_transactions**: List recent exit transactions and revenue logs
- **update_tariff**: Use this to adjust hourly rates or caps.

Update tariff rules or rates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IP Parking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the occupancy of Site A."

**🤖 AI Agent:**
> Site A: 142 available spaces out of 200 (71% full). Today's revenue: €1,250.

---

**👤 You:**
> "Open gate 3 for a manual exit."

**🤖 AI Agent:**
> Gate 3 command sent: 'open'. Barrier is now open. Ticket cycle reset.

---

**👤 You:**
> "Update tariff 'Standard' to €4.50 per hour."

**🤖 AI Agent:**
> Tariff 'Standard' updated successfully. New rate: €4.50/hr. All ticket machines synchronized.


## ❓ FAQ

**Q: Can I remotely open a barrier for a customer?**
Yes! Use the control_gate action with the gate_id and action 'open'. This is essential for remote assistance when ticket machines fail.

**Q: How do I check the current occupancy of a site?**
Use get_site_status with the site_id. It returns the number of available spaces versus total capacity and today's revenue.

**Q: Can I update hourly rates on the fly?**
Yes! Use update_tariff with the tariff_id and the new rate_per_hour. Changes are usually applied immediately to the ticket dispensers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ip-parking](https://vinkius.com/mcp/ip-parking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IP Parking** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ip-parking` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IP Parking** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ip-parking": {
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
