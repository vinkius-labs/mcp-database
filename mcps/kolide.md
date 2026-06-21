# Kolide MCP Server

Audit fleet security — list devices, track issues, and monitor people.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/kolide)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 10

## Description
Connect your AI agent to **Kolide** to get full visibility into your organization's fleet security and device health.

### Key Features

- **Fleet Inventory** — List all managed devices and their high-level security status
- **Issue Tracking** — Monitor active security vulnerabilities and misconfigurations across your fleet
- **People & Ownership** — See which users are associated with which devices and their individual compliance state
- **Security Checks** — Audit available security checks and dive into specific failure conditions
- **Audit Logs** — Access a chronological history of administrative and security events

### How to setup

1. Subscribe to this server
2. Log in to Kolide, go to **Settings** > **API**, and generate a Bearer Token
3. Enter your token in the configuration
4. Start auditing your fleet via natural language


## Available Tools
- **list_kolide_devices**: Use this to audit fleet security posture and identify individual device IDs.

List all devices in the fleet
- **get_device_details**: Get details for a specific device
- **list_kolide_issues**: List security issues across the fleet
- **get_issue_details**: Get details for a specific security issue
- **list_kolide_people**: List people/users managed in Kolide
- **get_person_details**: Get details for a specific person
- **list_kolide_checks**: List all available security checks
- **get_check_details**: Get details for a specific check
- **list_kolide_audit_logs**: List fleet audit logs
- **get_kolide_fleet_stats**: g., total devices, online status, issue count).

Get high-level fleet statistics


## Installation & Usage

To install and use the **Kolide** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kolide](https://vinkius.com/mcp/kolide)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
