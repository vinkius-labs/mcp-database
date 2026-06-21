# Balena MCP Server

Manage IoT fleets and edge devices via Balena — list devices, manage environment variables, and track releases directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/balena)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Balena** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/balena](https://vinkius.com/mcp/balena)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
