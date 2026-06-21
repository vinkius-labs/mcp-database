# Balena MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/balena)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/balena-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/balena-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Manage IoT fleets and edge devices via Balena — list devices, manage environment variables, and track releases directly from your AI agent.

## Description
Connect your **BalenaCloud** account to any AI agent to orchestrate your IoT infrastructure through natural language. Monitor device health, manage fleet configurations, and handle deployments without leaving your chat interface.

### What you can do

- **Fleet & Device Monitoring** — List all fleets (applications) and query specific devices using OData filters for precise status updates.
- **Configuration Management** — Dynamically create device-specific environment variables and metadata tags to organize your edge hardware.
- **Release Tracking** — Inspect deployment history and releases across your organizations to ensure your fleet is running the correct software.
- **OS Provisioning** — Query available balenaOS versions for specific device types and retrieve direct download URLs for rapid prototyping.
- **Identity Management** — Verify your current user profile, organizations, and active API keys associated with your account.

### How it works

1. Subscribe to this server
2. Enter your Balena API Key
3. Start managing your edge infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **IoT Engineers** — quickly check device statuses or logs without navigating the BalenaCloud dashboard.
- **DevOps Teams** — automate environment variable updates and release inspections during deployment cycles.
- **Product Owners** — get high-level overviews of fleet health and organization-wide project statuses.


## Available Tools
- **list_api_keys**: List Balena API keys
- **create_device_env_var**: Create a device environment variable
- **create_device_tag**: Create a device tag
- **list_devices**: Use OData $filter, $select, and $expand for advanced querying (e.g., $filter=uuid eq '<UUID>').

List devices in Balena fleets
- **list_fleets**: Use OData $filter, $select, and $expand for advanced querying (e.g., $filter=slug eq '<SLUG>').

List Balena fleets (applications)
- **get_os_download_url**: Get the download URL for a balenaOS image
- **list_os_versions**: g., raspberrypi3).

List available balenaOS versions for a device type
- **list_organizations**: List Balena organizations
- **list_releases**: Use OData $filter to filter by fleet (e.g., $filter=belongs_to__application eq <FLEET_ID>).

List Balena releases
- **whoami**: Get current Balena user details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Balena** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Balena fleets and their associated IDs."

**🤖 AI Agent:**
> I've retrieved your fleets. You have 3 active fleets: 'Smart-Home-Gateway' (ID: 18234), 'Industrial-Sensor-Node' (ID: 19455), and 'Edge-AI-Camera' (ID: 20112).

---

**👤 You:**
> "Add a tag 'location' with value 'warehouse-north' to device 1234567."

**🤖 AI Agent:**
> Successfully created the tag 'location: warehouse-north' for device 1234567. The device metadata has been updated.

---

**👤 You:**
> "What are the available balenaOS versions for a raspberrypi4-64?"

**🤖 AI Agent:**
> I found several versions for raspberrypi4-64. The latest stable releases include v2.115.18, v2.113.18, and v2.108.27. Would you like the download URL for any of these?


## Installation & Usage

To install and use the **Balena** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/balena](https://vinkius.com/mcp/balena)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
