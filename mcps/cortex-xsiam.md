# Cortex XSIAM MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cortex-xsiam)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cortex-xsiam-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cortex-xsiam-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [other](../categories/other.md)

Connect Cortex XSIAM to any AI agent via MCP.



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

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
