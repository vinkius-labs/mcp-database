# Cortex XSIAM MCP Server

Connect Cortex XSIAM to any AI agent via MCP.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cortex-xsiam)

## Overview
**Category:** other
**Tools Count:** 9



## Available Tools
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

To install and use the **Cortex XSIAM** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cortex-xsiam](https://vinkius.com/mcp/cortex-xsiam)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
