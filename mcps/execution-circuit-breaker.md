# Execution Circuit Breaker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/execution-circuit-breaker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [reliability](../categories/reliability.md)

Prevent cascading failures by monitoring consecutive errors and managing execution permissions.

## Description
The Execution Circuit Breaker is a stability pattern designed to prevent an agent from repeatedly attempting operations that are likely to fail. By tracking consecutive failures, it can trip the circuit to an OPEN state, blocking all calls for a cooldown period. Use `get_circuit_status` to check if execution is permitted, `record_success` to reset failure counts when tasks succeed, and `record_failure` to increment error tallies when operations fail.


## Available Tools (3)
- **get_circuit_status**: Determines the current operational state of the circuit and whether execution is permitted
- **record_failure**: Notifies the circuit breaker that an execution attempt failed
- **record_success**: Notifies the circuit breaker that an execution attempt was successful


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Execution Circuit Breaker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the current status of the circuit breaker at tick 100."

**🤖 AI Agent:**
> The circuit is currently in the CLOSED state, and execution is permitted (shouldExecute: true).

---

**👤 You:**
> "I just encountered an error while running a tool at tick 105. How should I update the circuit?"

**🤖 AI Agent:**
> You should call `record_failure` with `currentTick: 105`. If this failure reaches the threshold, the circuit will transition to OPEN.

---

**👤 You:**
> "The task completed successfully at tick 110. Update the registry."

**🤖 AI Agent:**
> You should call `record_success` with `currentTick: 110`. This will reset the consecutive failure count to zero and potentially close the circuit if it was in HALF_OPEN.


## ❓ FAQ

**Q: What does it mean when the circuit is in an OPEN state?**
An OPEN state means the failure threshold has been reached, and all execution attempts are currently blocked to allow for a cooldown period.

**Q: How can I check if I am allowed to execute a task?**
You should use the `get_circuit_status` tool. It will return whether the state is CLOSED, OPEN, or HALF_OPEN and provide a `shouldExecute` flag.

**Q: Does this system use real-world time?**
No, the system uses a deterministic integer-based tick counter to ensure all state transitions are perfectly reproducible in testing environments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/execution-circuit-breaker](https://vinkius.com/mcp/execution-circuit-breaker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Execution Circuit Breaker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `execution-circuit-breaker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Execution Circuit Breaker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "execution-circuit-breaker": {
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
