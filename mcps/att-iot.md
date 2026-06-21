# AT&T IoT MCP Server

IoT Control Center -- Manage SIM devices, activation, data pools, shared plans, and connectivity diagnostics via AT&T IoT API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/att-iot)

## Overview
**Category:** industry-titans
**Tools Count:** 10

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


## Available Tools
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


## Installation & Usage

To install and use the **AT&T IoT** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/att-iot](https://vinkius.com/mcp/att-iot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
