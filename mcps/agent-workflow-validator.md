# Agent Workflow Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-workflow-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Validates the structural integrity, metrics, and constraints of deterministic finite state machine workflows.

## Description
This MCP server provides a suite of tools to validate agentic workflows modeled as directed graphs. It ensures workflows are structurally sound by checking reachability and dead-ends using `validate_workflow_structure`. It calculates path complexity and visit frequencies via `analyze_workflow_metrics`, and enforces business logic like decision completeness and timeout coverage through `check_workflow_constraints`. It is designed to ensure deterministic behavior in complex agentic state machines.


## Available Tools (3)
- **validate_workflow_structure**: Performs a fundamental structural integrity check on the state machine topology
- **analyze_workflow_metrics**: Calculates statistical properties and complexity of the workflow paths
- **check_workflow_constraints**: Validates specific business logic constraints like decision completeness and timeout coverage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Workflow Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate the structure of this workflow: states=[{'stateId': 's1', 'type': 'start'}, {'stateId': 's2', 'type': 'end'}], transitions=[{'fromStateId': 's1', 'toStateId': 's2'}]"

**🤖 AI Agent:**
> {"is_valid": true, "unreachable_state_ids": [], "dead_end_state_ids": [], "errors": []}

---

**👤 You:**
> "Check the constraints for a decision state where probabilities don't sum to 1."

**🤖 AI Agent:**
> {"decision_completeness_valid": false, "timeout_coverage_pct": 0, "invalid_decision_states": ["decision_state_id"]}

---

**👤 You:**
> "Calculate the metrics for my workflow."

**🤖 AI Agent:**
> {"min_path_length": 2, "max_path_length": 2, "max_path_exceeded": false, "state_visit_frequencies": {"start": 1.0, "end": 1.0}}


## ❓ FAQ

**Q: What does `validate_workflow_structure` check?**
It verifies that there is exactly one start state, identifies unreachable states, and flags dead-end states that lack outgoing transitions.

**Q: How can I check if my decision states are valid?**
Use the `check_workflow_constraints` tool. It validates that the sum of probabilities for all exit conditions in a decision state equals exactly 1.0.

**Q: Can this tool handle complex workflows?**
Yes, `analyze_workflow_metrics` can calculate path lengths and visit frequencies, and it will flag any workflow where the maximum path length exceeds 50 states.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-workflow-validator](https://vinkius.com/ai-agent-connect/agent-workflow-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Workflow Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-workflow-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Workflow Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-workflow-validator": {
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
