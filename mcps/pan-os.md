# PAN-OS MCP Server

Connect PAN-OS to any AI agent via MCP.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pan-os)

## Overview
**Category:** other
**Tools Count:** 8



## Available Tools
- **commit**: This validates the config and activates it. Returns the commit job ID and status. Use this after making configuration changes to activate them.

Commit the candidate configuration to running configuration
- **get_active_sessions**: Use this to monitor real-time activity, identify heavy users, or debug connection issues.

List all active network sessions on the firewall
- **get_nat_rules**: Use this to audit NAT configurations or troubleshoot connectivity issues.

List all NAT rules configured on the firewall
- **get_pending_changes**: Use this to verify if the running configuration matches the candidate configuration before committing.

Check if there are uncommitted configuration changes
- **get_security_rules**: Use this to audit firewall policies, review access controls, or analyze rule usage.

List all security rules configured on the firewall
- **get_system_info**: Use this to verify firewall health, check software versions, or confirm connectivity.

Get system information and status of the PAN-OS firewall
- **get_threat_logs**: Contains source/dest IPs, threat names, severity, actions taken, and PCAP availability. Use this to investigate security incidents or analyze attack vectors.

Retrieve recent threat logs from the firewall
- **get_traffic_logs**: Optional limit parameter controls number of logs returned. Use this to analyze traffic patterns, identify blocked connections, or troubleshoot network issues.

Retrieve recent traffic logs from the firewall


## Installation & Usage

To install and use the **PAN-OS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pan-os](https://vinkius.com/mcp/pan-os)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
