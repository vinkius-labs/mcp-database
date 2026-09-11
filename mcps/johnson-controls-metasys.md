# Johnson Controls Metasys MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/johnson-controls-metasys)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Johnson Controls Metasys building automation as an MCP: browse the object tree, live alarms with annotations, equipment, network devices and spaces — official REST API v4 with bearer JWT auth.

## Description
**Metasys** — Johnson Controls' building automation system (BAS) — and its official REST API v4 as a single MCP server.

### What you can do
- **Browse the object tree** — every device, point and node on the site, with attributes, present values and hierarchy children
- **Alarms** — live and historical alarms (fire, security, HVAC) with operator annotations
- **Equipment** — chillers, AHUs, RTUs with their pointsUrl
- **Network devices** — controllers (NAE, MBC...) with firmware and topology
- **Spaces** — rooms, zones and floors for comfort monitoring
- **Activities & audits** — who changed what, and when

### Authentication (from the official Metasys REST API docs)
1. Requires a Metasys Site (v11+) with the REST API enabled and an account whose **Access Type is "API"** (Active Directory accounts: `{name}@{domain}`)
2. The MCP logs in at `POST /api/v4/login` and receives a Bearer **JWT access token**
3. Token expiry follows the Metasys profile — the official guidance is to refresh before 60 minutes, which this MCP does automatically

### Who is this for?
Building operations teams, energy managers, fault-detection analytics, systems integrators and AI agents monitoring JCI/Metasys buildings.


## Available Tools (8)
- **get_object**: ), object type, and URLs for children/alarms. Use UUIDs from list_objects.

Get one Metasys object: attributes, present values, status and hierarchy links
- **list_objects**: Returns objectId (UUID) with name, description and type. Children of an object: get_object_children. Paging via page/size.

List Metasys objects (BACnet-ish tree: devices, points, equipment nodes)
- **get_object_children**: Children may be paginated via the returned pages links.

List the children of a Metasys object (browse down the building tree)
- **list_alarms**: Filter by object with the object query, or browse pages. Each alarm supports annotations (get via /alarms/{id}/annotations).

List Metasys alarms (fire, security, HVAC alarms across the site)
- **get_alarm_annotations**: Get operator annotations/notes on an alarm
- **list_equipment**: Equipment groups physical devices regardless of the network topology.

List equipment in the Metasys site (chillers, AHUs, RTUs...)
- **list_network_devices**: ) with firmware versions and their equipment/pointsUrl. The network topology view.

List network devices: controllers and field buses connected to Metasys
- **list_spaces**: Useful for comfort monitoring per room.

List spaces (rooms, zones, floors) with their temperature/humidity links


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Johnson Controls Metasys** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me active alarms in the building"

**🤖 AI Agent:**
> 🚨 **Metasys alarms (page 0)**

- AHU-3 Supply Fan Failure — alarm, 2026-09-07 06:14
- Chiller 1 Low Refrigerant — alarm, 2026-09-06 22:41
- VAV-201 Temperature High — warning, ongoing

2 have operator annotations. Want the full attribute detail of any alarm?

---

**👤 You:**
> "Browse what devices are on my Metasys site"

**🤖 AI Agent:**
> 🌳 **Metasys object tree (page 0)**

Root: Building A → NAE-1 (network device) → AHU-1, VAV-101..VAV-230, FCU devices...

Each node exposes children via get_object_children — I can walk down to individual sensor points and read their present values.

---

**👤 You:**
> "What equipment do I have and which controllers manage them?"

**🤖 AI Agent:**
> ⚙️ **Equipment & network devices**

Equipment: Chiller-1, AHU-2, Boiler-1 (each with pointsUrl)
Network devices: NAE-1 (v9.0.2), MBC-B1 (v14.1) — with firmware versions

I can map each equipment to its managing controller and pull any point's present value.


## ❓ FAQ

**Q: What do I need on my Metasys site for this to work?**
A Metasys Site (ADS/OTI server) running Metasys v11+ with the REST API enabled, and an account whose Access Type is set to 'API' (created in the Metasys UI). Active Directory users format the username as name@domain.

**Q: Does the token expire?**
Yes — JWT expiry follows the Metasys profile. The official guidance is to refresh before 60 minutes; this MCP refreshes the token at 55 minutes automatically, so long monitoring sessions keep working.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/johnson-controls-metasys](https://vinkius.com/en/ai-agent-connect/johnson-controls-metasys)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Johnson Controls Metasys** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `johnson-controls-metasys` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Johnson Controls Metasys** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "johnson-controls-metasys": {
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
