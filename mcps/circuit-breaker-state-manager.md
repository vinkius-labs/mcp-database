# Circuit Breaker State Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/circuit-breaker-state-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Prevents cascading failures by managing service health states.

## Description
This MCP server provides a robust mechanism to protect agentic workflows from failing downstream dependencies. By implementing the circuit breaker pattern, it monitors service health and automatically transitions between CLOSED, OPEN, and HALF_OPEN states. Use `get_circuit_status` to monitor service health, `record_result` to update the state after service calls, and `configure_circuit` to adjust failure thresholds or cooldown periods. This ensures that your AI agents do not waste resources on failing services and can automatically recover when services become stable again.


## Available Tools (3)
- **configure_circuit**: Change the sensitivity or behavior of the circuit breaker for a specific service
- **get_circuit_status**: Get the current health and status of the circuit breaker
- **record_result**: Update the circuit breaker based on the outcome of a service call


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Circuit Breaker State Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the LLM service currently healthy?"

**🤖 AI Agent:**
> The current status for the LLM service is CLOSED, and calls are permitted.

---

**👤 You:**
> "The external API just failed. How should I update the circuit breaker?"

**🤖 AI Agent:**
> You should call `record_result` with `isSuccess` set to false for that service ID.

---

**👤 You:**
> "What is the remaining cooldown time for the database service?"

**🤖 AI Agent:**
> The database service is currently in the OPEN state with 45000ms remaining until it enters the HALF_OPEN state.


## ❓ FAQ

**Q: What is the purpose of the circuit breaker?**
It prevents cascading failures by stopping requests to a service that is currently failing, allowing it time to recover.

**Q: How do I check if a service is currently blocked?**
You can use the `get_circuit_status` tool to check the current state and see if `allowCall` is true.

**Q: Can I customize the failure threshold?**
Yes, use the `configure_circuit` tool to set a custom `failureThreshold` for any specific service.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/circuit-breaker-state-manager](https://vinkius.com/mcp/circuit-breaker-state-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Circuit Breaker State Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `circuit-breaker-state-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Circuit Breaker State Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "circuit-breaker-state-manager": {
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
