# Saga Compensation Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/saga-compensation-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [reliability](../categories/reliability.md)

Orchestrates deterministic recovery paths for distributed transactions using the Saga pattern.

## Description
This MCP server provides a deterministic orchestration engine for managing distributed transactions via the Saga pattern. When a multi-agent transaction fails, this tool calculates the exact reverse-order compensation sequence required to revert the system to a consistent state. It determines the necessary compensation steps, calculates total recovery time, and evaluates the final saga state (such as COMPENSATED or REQUIRES_MANUAL_INTERVENTION). Use `plan_compensation_sequence` to map out recovery paths, `get_saga_metadata` to retrieve correlation IDs and idempotency keys, and `evaluate_saga_status` to assess the outcome of compensation attempts.


## Available Tools (3)
- **evaluate_saga_status**: Determines the high-level status of the transaction based on the outcome of the compensation attempts
- **get_saga_metadata**: Retrieves the unique tracking identifiers used to maintain the lifecycle of the specific saga instance
- **plan_compensation_sequence**: Calculates the exact order of compensation actions and the total projected time required to revert the transaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Saga Compensation Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the compensation plan for a saga where the failure occurred at step index 2, given these steps: [{stepId: '1', agentId: 'A', action: 'reserve', compensationAction: 'cancel', timeoutMs: 500}, {stepId: '2', agentId: 'B', action: 'pay', compensationAction: 'refund', timeoutMs: 1000}]"

**🤖 AI Agent:**
> The compensation sequence will execute 'refund' for step 2, then 'cancel' for step 1. The total compensation time is 1500ms.

---

**👤 You:**
> "What is the current status of a saga if all compensation attempts were successful?"

**🤖 AI Agent:**
> The saga state is COMPENSATED.

---

**👤 You:**
> "How do I get the idempotency keys for my saga steps?"

**🤖 AI Agent:**
> You can use the `get_saga_metadata` tool to retrieve the unique stepIdempotencyKeys for each step in your saga.


## ❓ FAQ

**Q: What is the purpose of the compensation sequence?**
The compensation sequence provides the exact, reverse-order list of actions needed to undo successful steps after a transaction failure, ensuring system consistency.

**Q: How does the tool handle a failure during the compensation phase?**
If a compensation action fails, the tool identifies the state as FAILED_COMPENSATION or REQUIRES_MANUAL_INTERVENTION to alert the system that automated recovery could not be completed.

**Q: Can I use this to track transactions across multiple agents?**
Yes, by using `get_saga_metadata`, you can retrieve the correlation ID used to trace the transaction across all participating agents.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/saga-compensation-planner](https://vinkius.com/ai-agent-connect/saga-compensation-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Saga Compensation Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `saga-compensation-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Saga Compensation Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "saga-compensation-planner": {
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
