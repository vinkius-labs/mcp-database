# Hologram.io MCP Server

Automate IoT connectivity via Hologram.io — manage devices, SIM cards, and data usage directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/hologramio)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 11

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


## Installation & Usage

To install and use the **Hologram.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hologramio](https://vinkius.com/mcp/hologramio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
