# PAN-OS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pan-os)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [other](../categories/other.md)

Connect PAN-OS to any AI agent via MCP.



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

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pan-os](https://vinkius.com/mcp/pan-os)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PAN-OS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pan-os` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PAN-OS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pan-os": {
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
