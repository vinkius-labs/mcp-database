# Prisma Access MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/prisma-access)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [other](../categories/other.md)

Connect Prisma Access to any AI agent via MCP.



## Available Tools (7)
- **get_locations**: Use this to review network topology or troubleshoot routing.

List mobile user locations and remote networks
- **get_policies**: Use this to audit SASE policies.

List security policies enforced in Prisma Access
- **get_service_endpoints**: Use this to verify regional connectivity or configure DNS routing.

List Prisma Access service endpoints (PoPs)
- **get_threat_logs**: Includes severity, attack details, and action taken. Use this to investigate attacks against remote endpoints.

Retrieve recent threat detection logs from Prisma Access
- **get_traffic_logs**: Use this to analyze usage patterns or debug access issues.

Retrieve recent network traffic logs from Prisma Access
- **get_tunnels**: Use this to monitor network connectivity and troubleshoot tunnel drops.

List SD-WAN and network tunnels in Prisma Access
- **get_users**: Use this to audit remote work access or identify inactive accounts.

List remote users connected to Prisma Access






## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/prisma-access](https://vinkius.com/mcp/prisma-access)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Prisma Access** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `prisma-access` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Prisma Access** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "prisma-access": {
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
