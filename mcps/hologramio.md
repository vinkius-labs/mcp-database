# Hologram.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hologramio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Automate IoT connectivity via Hologram.io — manage devices, SIM cards, and data usage directly from any AI agent.

## Description
Connect your **Hologram.io** IoT platform to any AI agent and take full control of your global cellular connectivity and device fleet through natural conversation.

### What you can do

- **Device Oversight** — List all IoT devices in your account, retrieve detailed metadata, and monitor their active status.
- **SIM Card Management** — Access lists of SIM cards (cellular links) and their associated data plans to ensure seamless connectivity.
- **Data Usage Monitoring** — Retrieve recent data sessions, daily usage statistics, and current billing cycle summaries.
- **Connectivity Control** — Quickly pause or unpause data services for specific SIM cards directly from the chat interface.
- **Location Insights** — Access approximate GPS coordinates for your entire fleet based on cell tower triangulation.
- **SMS Tracking** — Retrieve the history of device-originated SMS messages for troubleshooting and logging.

### How it works

1. Subscribe to this server
2. Enter your Hologram API Key (found in Dashboard > API)
3. Start managing your IoT fleet from Claude, Cursor, or any MCP-compatible client

No more manual exporting of usage logs or jumping between complex fleet management screens. Your AI assistant acts as a dedicated IoT Operations Manager or Network Specialist.

### Who is this for?

- **IoT Engineers** — instantly check device connectivity and retrieve data session logs during development.
- **Fleet Managers** — automate the process of monitoring data overages and pausing inactive SIMs.
- **Operations Leads** — maintain a real-time overview of fleet location and billing usage.


## Available Tools
- **get_billing_cycle_usage**: Check data usage for the current billing cycle
- **get_daily_usage_stats**: Retrieve aggregated daily data usage statistics
- **get_device_details**: Get detailed information for a specific IoT device
- **get_device_locations**: Retrieve approximate GPS coordinates for all devices based on cell tower data
- **get_recent_data_sessions**: Retrieve the most recent data sessions for your fleet
- **list_available_data_plans**: List all data plans available for activation in your organization
- **list_iot_devices**: Use this to monitor fleet status and find specific device IDs.

List all IoT devices in your Hologram account
- **list_sim_cards**: List all SIM cards (cellular links) and their associated plans
- **list_sms_messages**: Retrieve the history of device-originated SMS messages
- **pause_sim_data**: Requires the cellular link ID.

Temporarily suspend data services for a specific SIM card
- **unpause_sim_data**: Resume data services for a suspended SIM card


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hologram.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all IoT devices and show which ones are currently active."

**🤖 AI Agent:**
> I've retrieved your device list. You have 12 devices in your fleet, including 'Sensor Unit 01' (Active), 'Gateway Beta' (Active), and 'Tracker 05' (Suspended). Would you like to see the recent data usage for the active devices?

---

**👤 You:**
> "Show me the total data usage for the current billing cycle."

**🤖 AI Agent:**
> Accessing billing usage... For the current cycle, your fleet has consumed 450.2 MB of data. Your monthly allowance is 1 GB, leaving you with 549.8 MB remaining. Should I check which device has the highest consumption?

---

**👤 You:**
> "Find the approximate location of all devices in my account."

**🤖 AI Agent:**
> Retrieving fleet locations... I've mapped your devices based on cell tower data. Most of your fleet is currently concentrated in the 'Greater Chicago Area', with 2 units appearing near 'San Francisco'. Would you like the specific coordinates for any device?


## ❓ FAQ

**Q: How do I find my Hologram.io API Key?**
Log in to your Hologram dashboard, click on your profile/organization name, navigate to **Settings**, and select the **API** tab. You will find your unique API Key there.

**Q: Can I pause data for a specific device?**
Yes! Use the `pause_sim_data` tool by providing the unique cellular link ID for that device. This will change its state to 'suspended' and stop data usage immediately.

**Q: How accurate is the device location feature?**
The location data provided by `get_device_locations` is approximate and based on cell tower triangulation. It is generally accurate within a few hundred meters to a few miles depending on tower density.

**Q: Is the integration secure for managing my IoT fleet?**
Absolutely. The integration uses industry-standard Basic Authentication over HTTPS. Your credentials and connectivity data are encrypted and stored securely within the Vinkius Cloud infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hologramio](https://vinkius.com/mcp/hologramio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hologram.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `hologramio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hologram.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hologramio": {
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
