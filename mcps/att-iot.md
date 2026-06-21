# AT&T IoT MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/att-iot)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

IoT Control Center -- Manage SIM devices, activation, data pools, shared plans, and connectivity diagnostics via AT&T IoT API.

## Description
Connect your **AT&T IoT** account to any AI agent and take full command of your IoT SIM fleet through natural conversation.

### What you can do

- **Device Inventory** -- List all IoT SIMs with ICCIDs, statuses (active, suspended, deactivated), data plan names, and last activity dates
- **Real-Time Status** -- Get live connectivity state, IP address, signal strength, data used/remaining, and suspension reasons for any SIM
- **Activate & Suspend** -- Instantly activate suspended devices or suspend compromised SIMs to block network access and contain costs
- **Resume Devices** -- Restore network access to suspended SIMs after troubleshooting or policy clearance without reprovisioning
- **Data Usage Tracking** -- Retrieve current and historical usage per SIM with daily breakdowns, overage alerts, and cycle forecasts
- **Data Pool Management** -- List shared data pools, monitor aggregate consumption, identify top-consuming devices, and prevent pool exhaustion
- **Device Configuration** -- Update rate limits, APN settings, and pool assignments to optimize performance or migrate devices between plans
- **Automated Diagnostics** -- Run connectivity troubleshooting checks including network registration, APN config, data session status, and known outages

### How it works

1. Subscribe to this server
2. Enter your AT&T IoT API Key and Client ID
3. Start managing your IoT fleet from Claude, Cursor, or any MCP-compatible client

No more logging into the IoT Control Center portal for every SIM check. Your AI agent becomes your IoT operations console.

### Who is this for?

- **IoT Fleet Managers** -- monitor device health at scale, track data pool consumption, and prevent SIM exhaustion before it happens
- **Field Engineers** -- diagnose offline devices remotely, activate new deployments, and suspend lost or stolen SIMs instantly
- **Network Operations** -- troubleshoot connectivity issues with automated diagnostics, review APN configurations, and check known outages
- **Finance Teams** -- audit data usage across the fleet, forecast billing cycles, and reallocate unused pool capacity to save costs


## Available Tools (10)
- **activate_device**: Returns activation timestamp and assigned IP. Use to onboard new devices or restore service after maintenance.

Activate a suspended or deactivated IoT SIM
- **diagnose_connectivity**: Returns diagnostic results and recommended actions. Use for rapid troubleshooting of offline devices.

Run automated diagnostics to troubleshoot IoT device connectivity
- **get_data_usage**: Use to monitor plan limits, identify heavy users, or forecast billing.

Retrieve current and historical data usage for an IoT SIM
- **get_device_status**: Use to troubleshoot offline devices or verify data allowance.

Get real-time connectivity and data status of an IoT SIM
- **get_pool_usage**: Use to prevent pool exhaustion or reallocate unused data.

Get detailed usage metrics for a specific data pool
- **list_data_pools**: Use to manage enterprise data sharing across fleets.

List shared data pools configured for IoT devices
- **list_devices**: Use to audit fleet inventory, identify inactive SIMs, or verify provisioning status.

List all IoT SIMs/devices managed in AT&T Control Center
- **resume_device**: Use to restore service after troubleshooting or policy clearance.

Resume network access for a suspended IoT SIM
- **suspend_device**: Use for lost/stolen devices, cost containment, or decommissioning.

Suspend an IoT SIM to block network access
- **update_device_settings**: Requires ICCID and JSON settings object. Use to optimize performance or migrate devices between plans.

Update configuration settings for an IoT device


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AT&T IoT** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my IoT devices and show me which ones are suspended."

**🤖 AI Agent:**
> I've retrieved your IoT fleet inventory. Total devices: 247. Active: 231, Suspended: 14, Deactivated: 2. Here are the 14 suspended devices with their ICCIDs and suspension reasons: 3 devices suspended for exceeding data limits, 8 suspended manually (cost containment), 3 suspended due to reported loss/theft. Would you like me to resume any of the cost-containment suspensions?

---

**👤 You:**
> "Device ICCID 8901234567890123456 is offline. Run diagnostics and tell me what's wrong."

**🤖 AI Agent:**
> Diagnostics complete for ICCID 8901234567890123456. Issue identified: APN configuration mismatch. The device is registered on the network and has strong signal (-67 dBm), but the APN 'iot.att.net' is returning authentication failures. Recommended action: update the APN settings using `update_device_settings` with the correct APN value. No network outages reported in the device's area.

---

**👤 You:**
> "Check the data pool usage for 'Enterprise-Fleet-A' and tell me our top 5 consuming devices."

**🤖 AI Agent:**
> Pool 'Enterprise-Fleet-A' usage: 78.3 GB used out of 100 GB allocated (78.3%). 21.7 GB remaining. Renewal date: April 28. Top 5 consuming devices: 1) ICCID ...3456 (8.2 GB), 2) ICCID ...7891 (6.7 GB), 3) ICCID ...2345 (5.1 GB), 4) ICCID ...6789 (4.8 GB), 5) ICCID ...0123 (3.9 GB). At current rate, the pool will reach 90% by April 20. Consider suspending non-critical devices or reallocating capacity.


## ❓ FAQ

**Q: What information do I need to identify an IoT SIM?**
Each IoT SIM is uniquely identified by its **ICCID** (Integrated Circuit Card Identifier) -- a 19-20 digit number printed on the SIM card or available in your IoT Control Center dashboard. The ICCID is required for all device-specific operations like activation, suspension, and usage queries. You can list all your devices with `list_devices` to discover ICCIDs for your entire fleet.

**Q: How do data pools work and how can I prevent pool exhaustion?**
Data pools are shared data plans across multiple IoT SIMs. Instead of each SIM having an individual cap, all devices in the pool draw from a common data bucket. Use `list_data_pools` to see your pools, `get_pool_usage` to check consumption and identify top-consuming devices, and set up alerts before reaching the limit. If a pool is near exhaustion, you can suspend low-priority devices with `suspend_device` or migrate high-usage devices to a different pool with `update_device_settings`.

**Q: Can I automatically diagnose why an IoT device went offline?**
Yes. Use the `diagnose_connectivity` tool with the device's ICCID. It runs automated checks for network registration status, APN configuration, active data session, signal strength, and known network outages in the device's area. The tool returns detailed diagnostic results with recommended actions -- helping your field engineers resolve connectivity issues without manual portal navigation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/att-iot](https://vinkius.com/mcp/att-iot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AT&T IoT** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `att-iot` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AT&T IoT** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "att-iot": {
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
