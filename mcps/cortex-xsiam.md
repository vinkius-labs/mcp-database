# Cortex XSIAM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cortex-xsiam)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [other](../categories/other.md)

Connect Cortex XSIAM to any AI agent via MCP.



## Available Tools (9)
- **execute_playbook**: g., enrich IOCs, block IP, reset password). Requires playbook name and optional input arguments. Use this to speed up response times and ensure consistent handling of incidents.

Execute an automated incident response playbook in Cortex XSIAM
- **get_alerts**: Use this to review detection rules firing or analyze threat patterns.

List security alerts detected by Cortex XSIAM
- **get_endpoints**: Use this to audit endpoint coverage, identify disconnected hosts, or target remediation actions.

List managed endpoints (hosts/devices) in Cortex XSIAM
- **get_incident_details**: Requires the incident ID. Use this for deep investigation or context before taking action.

Get detailed information about a specific security incident
- **get_incidents**: Use this to monitor SOC queue, identify high-severity incidents, or track analyst workload. Supports sorting and limiting results.

List security incidents in Cortex XSIAM
- **get_indicators**: Use this to review threat intelligence or check if specific artifacts are known malicious.

List indicators of compromise (IOCs) tracked in Cortex XSIAM
- **isolate_endpoint**: Requires the endpoint ID. Use this immediately upon confirming a severe compromise to prevent lateral movement.

Isolate a compromised endpoint from the network
- **run_xql_query**: XQL allows searching logs, endpoints, network data, and more. Requires a valid XQL query string. Returns the results of the query. Use this for custom threat hunting, compliance reporting, or data analysis.

Execute an XQL (Cortex Query Language) query for advanced threat hunting
- **scan_endpoint**: Supports "quick" or "deep" scan types. Requires the endpoint ID. Use this to verify if a host is infected or after cleaning a threat.

Trigger a malware scan on a specific endpoint






## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cortex-xsiam](https://vinkius.com/mcp/cortex-xsiam)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cortex XSIAM** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cortex-xsiam` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cortex XSIAM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cortex-xsiam": {
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
