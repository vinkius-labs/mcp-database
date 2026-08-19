# Agent Load Balancer Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-load-balancer-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Deterministic load balancing engine for distributing request rates across agent instances.

## Description
This MCP server provides a deterministic engine to distribute incoming request rates across a pool of healthy agent instances. It supports multiple mathematical strategies including `round_robin`, `least_connections`, `weighted_response_time`, and `consistent_hashing`. Use `calculate_distribution` to determine exact request assignments, `get_sticky_session_mapping` for session persistence, and `analyze_system_health` to monitor pool utilization and imbalance ratios.


## Available Tools (3)
- **get_sticky_session_mapping**: Determines which specific instance a specific user/request will be routed to, simulating session persistence
- **analyze_system_health**: Provides a high-level overview of how stressed the agent pool is without performing a full distribution calculation
- **calculate_distribution**: Calculates exactly how many requests from the incoming rate should be assigned to each healthy agent instance based on the selected strategy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Load Balancer Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the request distribution for 100 requests/sec using least_connections across three instances: ID1 (load 10, cap 50), ID2 (load 20, cap 50), and ID3 (load 5, cap 50)."

**🤖 AI Agent:**
> The requests are distributed as follows: ID3 receives 100 requests because it has the lowest utilization ratio (0.1).

---

**👤 You:**
> "What is the current health status of my agent pool?"

**🤖 AI Agent:**
> The average utilization is 45%, the maximum utilization is 85%, and there are 0 unhealthy instances.

---

**👤 You:**
> "Map user 'user_123' to an instance using consistent hashing."

**🤖 AI Agent:**
> User 'user_123' is mapped to instance ID2.


## ❓ FAQ

**Q: How does the least_connections strategy work?**
The `least_connections` strategy assigns requests to the instance with the lowest ratio of current load to its total capacity.

**Q: Can I ensure a user always hits the same instance?**
Yes, by using the `consistent_hashing` strategy with a specific request ID or user ID, you can achieve sticky session routing.

**Q: How are unhealthy instances handled?**
All calculations, including `analyze_system_health`, automatically ignore any instances where the health status is false.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-load-balancer-calculator](https://vinkius.com/ai-agent-connect/agent-load-balancer-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Load Balancer Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-load-balancer-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Load Balancer Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-load-balancer-calculator": {
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
