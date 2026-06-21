# Umbrellar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/umbrellar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Cloud hosting, domains, and managed IT services.

## Description
The Umbrellar MCP server provides a direct conversational link to your cloud infrastructure. Query server status, check domain availability, and monitor your managed services directly via AI.


## Available Tools (12)
- **check_product_eligibility**: Check if a product is eligible for warranty coverage
- **create_claim**: Submit a new warranty claim
- **get_claim**: Get details for a specific warranty claim
- **get_policy**: Get details for a specific warranty policy
- **get_warranty**: Get details for a specific warranty plan
- **list_claims**: List all warranty claims
- **list_policies**: List all warranty policies
- **list_warranties**: List all available warranty plans
- **register_product**: Register a product for OEM or manufacturer warranty
- **sync_products**: Sync products between Shopify and Umbrellar
- **update_claim**: Update an existing warranty claim
- **validate_policy**: Validate if a policy exists by matching ID and order name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Umbrellar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active cloud servers."

**🤖 AI Agent:**
> You have 2 active servers: 'Web-Node-1' (Running) and 'DB-Master' (Running).

---

**👤 You:**
> "Check the expiration date for the domain 'vinkius.com'."

**🤖 AI Agent:**
> The domain 'vinkius.com' is active and will expire on October 14th, 2027.

---

**👤 You:**
> "Show the resource usage for 'Web-Node-1'."

**🤖 AI Agent:**
> 'Web-Node-1' is currently using 45% CPU, 2.1GB of RAM, and 40GB of disk space.


## ❓ FAQ

**Q: Can I check the uptime status of my virtual machines?**
Yes, just supply the VM ID and the agent will return its current operational status.

**Q: How do I query my registered domains?**
Ask the AI to list all your domains, and it will fetch their expiration dates and current configurations.

**Q: Is it possible to reboot a server through the chat?**
Server alteration commands like rebooting are disabled by default for safety, focusing the integration on observability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/umbrellar](https://vinkius.com/mcp/umbrellar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Umbrellar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `umbrellar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Umbrellar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "umbrellar": {
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
