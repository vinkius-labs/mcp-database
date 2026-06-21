# Prisma Cloud MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/prisma-cloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/prisma-cloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/prisma-cloud-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [other](../categories/other.md)

Connect Prisma Cloud to any AI agent via MCP.



## Available Tools
- **get_alerts**: Use this to identify misconfigurations or security risks in cloud resources.

List active security alerts in Prisma Cloud
- **get_cloud_accounts**: Use this to audit cloud inventory and verify onboarding status.

List all cloud accounts onboarded in Prisma Cloud
- **get_compliance**: Returns failing checks and remediation steps. Use this to audit cloud security posture and ensure regulatory compliance.

Check cloud compliance status against benchmarks (CIS, etc)
- **get_network_anomalies**: Use this to identify compromised workloads or insider threats.

Detect network anomalies and unusual traffic patterns in the cloud
- **get_policies**: Use this to review security rules enforced across cloud environments.

List all security policies configured in Prisma Cloud
- **get_user_profile**: Use this to verify API access levels or troubleshoot permissions.

Get profile information for the authenticated Prisma Cloud user
- **run_rql_query**: Requires a valid RQL string. Returns matching resources. Use this for custom compliance checks or hunting misconfigurations.

Execute a Resource Query Language (RQL) query for deep cloud analysis




## Installation & Usage

To install and use the **Prisma Cloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/prisma-cloud](https://vinkius.com/mcp/prisma-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
