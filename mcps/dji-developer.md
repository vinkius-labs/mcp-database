# DJI Developer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dji-developer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Orchestrate DJI drones and payloads — manage flight logs, monitor device health, and handle firmware updates directly from any AI agent.

## Description
Connect your AI agents to the **DJI Developer Platform**, the industry standard for unmanned aerial systems (UAS). This MCP provides 10 tools to manage enterprise drone fleets, monitor real-time telemetry logs, and orchestrate firmware lifecycle management for aircraft and payloads.

### What you can do

- **Fleet Monitoring** — List registered aircraft and payloads to track operational readiness and hardware versions
- **Flight Orchestration** — Retrieve detailed flight logs and telemetry data for post-mission analysis and compliance
- **Hardware Intelligence** — Get granular health reports and technical specifications for any device in your DJI ecosystem
- **Firmware Lifecycle** — Check for latest firmware releases and monitor the progress of remote updates programmatically
- **Resource Management** — Manage organization structures and retrieve pilot profiles linked to your developer account

### How it works

1. Subscribe to this server
2. Log in to the [**DJI Developer Center**](https://developer.dji.com/)
3. Register your application to obtain your **App ID** and **App Key**
4. Enable the **Cloud API** or **Enterprise API** for your devices
5. Insert your credentials into the fields below to start managing your DJI fleet operations.

### Who is this for?

- **Fleet Managers** — automate the tracking of aircraft health and flight compliance across multiple sites
- **Data Analysts** — integrate drone telemetry into broader GIS and operational reporting systems
- **DevOps Engineers** — monitor remote firmware deployments and device synchronization at scale


## Available Tools (10)
- **create_mission**: Create a new flight mission for a drone or dock
- **get_device_osd**: Retrieve real-time flight data (OSD)
- **get_device_status**: Get the online status and basic state of a drone
- **get_firmware_info**: Check firmware versions for a device
- **get_hms_stats**: Retrieve health management system (HMS) alerts
- **get_media_upload_url**: Request a cloud storage upload URL for media
- **get_mission_status**: Check the progress of an active flight mission
- **list_devices**: List all drones and docks bound to your account
- **list_media_files**: List photos and videos captured by a drone
- **list_waylines**: List available flight wayline files


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DJI Developer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all aircraft in my DJI fleet and show their firmware versions."

**🤖 AI Agent:**
> Retrieving DJI fleet data... I found 3 active aircraft: 1. Matrice 350 RTK (v01.02.03), 2. Mavic 3 Enterprise (v02.01.00), 3. Phantom 4 RTK (v01.05.06). Would you like to check if there are firmware updates for any of these?

---

**👤 You:**
> "What is the health status of aircraft SN 'DJI_SN_12345'?"

**🤖 AI Agent:**
> Querying DJI health diagnostics for SN 'DJI_SN_12345'... Status is 'Normal'. Battery cycle count is 45, current charge is 88%, and all internal sensors are operating within nominal parameters.

---

**👤 You:**
> "Show me the last flight log for the Mavic 3 Enterprise."

**🤖 AI Agent:**
> Fetching flight records... The last mission occurred on 2024-04-11. Total flight time: 24 minutes. Max altitude: 120m. GPS signal was stable throughout. Would you like the full telemetry export?


## ❓ FAQ

**Q: Can I automatically list all aircraft in my DJI fleet?**
Yes! Use the `list_aircraft` tool. Your agent will retrieve a complete list of all registered drones in your account, including their model names and current firmware versions.

**Q: How do I monitor the health status of a specific drone?**
Use the `get_device_health` tool with the aircraft serial number. The agent will return real-time health metrics, battery status, and any active error codes from the DJI platform.

**Q: Can I retrieve telemetry logs from past missions?**
Yes! Use the `get_flight_logs` tool. Your agent will fetch detailed historical flight data, including GPS coordinates, altitude, and velocity profiles for any recorded mission.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dji-developer](https://vinkius.com/mcp/dji-developer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DJI Developer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dji-developer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DJI Developer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dji-developer": {
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
