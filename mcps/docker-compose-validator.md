# Docker Compose Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/docker-compose-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Validate Docker Compose files for structural errors, port conflicts, and dependency cycles.

## Description
The Docker Compose Validator MCP server provides a specialized engine to audit your `docker-compose.yml` files. It identifies critical configuration errors before you run `docker compose up`, preventing runtime failures and deployment bottlenecks. Use tools like `validate_structure` to check YAML compliance, `detect_network_collisions` to find overlapping host ports, `audit_dependency_graph` to spot circular dependencies, and `verify_resource_integrity` to ensure all images and volumes are correctly defined.


## Available Tools (4)
- **audit_dependency_graph**: Detect circular startup chains and broken service references
- **detect_network_collisions**: Identify overlapping host port mappings
- **validate_structure**: yml file.

Validate the basic structural requirements of a Compose file
- **verify_resource_integrity**: Ensure services have valid sources and environment/volume references are sound


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Docker Compose Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this docker-compose file is valid: 'services:
  web:
    image: nginx
  db:
    image: postgres'"

**🤖 AI Agent:**
> The structure is valid. Both the web and db services are correctly defined with images.

---

**👤 You:**
> "Are there any port conflicts in these services: {"web": {"ports": ["80:80"]}, "proxy": {"ports": ["80:80"]}}?"

**🤖 AI Agent:**
> Yes, a collision was detected on host port 80 between the web and proxy services.

---

**👤 You:**
> "Check for broken dependencies in: {"web": ["db"], "db": ["redis"]}"

**🤖 AI Agent:**
> No circular paths or broken references were found in the dependency graph.


## ❓ FAQ

**Q: What can this MCP server validate?**
It validates YAML structure, detects host port collisions, audits dependency graphs for circular loops, and verifies resource integrity like images and volumes.

**Q: How do I check for port conflicts?**
You can use the `detect_network_collisions` tool by providing your service definitions as a JSON string.

**Q: Can it detect circular dependencies?**
Yes, the `audit_dependency_graph` tool specifically identifies loops in your service dependency chains.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docker-compose-validator](https://vinkius.com/mcp/docker-compose-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Docker Compose Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `docker-compose-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Docker Compose Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "docker-compose-validator": {
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
