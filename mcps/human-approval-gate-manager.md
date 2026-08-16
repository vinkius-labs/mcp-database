# Human Approval Gate Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/human-approval-gate-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Manages deterministic human-in-the-loop approval gates for agent actions.

## Description
This MCP server provides a deterministic engine for managing human-in-the-loop approval gates. It prevents workflow timeouts and excessive manual interruptions by applying risk-based thresholds to agent actions. Using `register_action`, you can submit tasks with specific risk levels (LOW, MEDIUM, HIGH, or CRITICAL). The system uses `check_action_status` to monitor the state of pending requests and `submit_human_decision` to allow manual intervention. For non-critical tasks, `refresh_gate_states` can be used to transition timed-out actions to an EXPIRED state based on your auto-approval rules. It is designed to bridge the gap between autonomous agentic workflows and necessary human oversight.


## Available Tools (4)
- **check_action_status**: Determines if a specific action is currently waiting, has been decided, or has expired
- **refresh_gate_states**: A maintenance tool to advance the state of all pending actions, specifically handling transitions to EXPIRED
- **register_action**: Submits a new action into the approval gate to start the monitoring process
- **submit_human_decision**: Allows a human user to manually approve or reject a pending action


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Human Approval Gate Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Register a new action to delete a database record with HIGH risk."

**🤖 AI Agent:**
> Action registered successfully with ID 'db_delete_001'. Status is currently PENDING.

---

**👤 You:**
> "What is the status of the action with ID 'task_123'?"

**🤖 AI Agent:**
> The action 'task_123' is currently PENDING and requires human input.

---

**👤 You:**
> "Approve the pending action 'auth_request_99'."

**🤖 AI Agent:**
> Decision submitted. Action 'auth_request_99' has been APPROVED.


## ❓ FAQ

**Q: How does the risk-based approval work?**
Every action is assigned a risk level. CRITICAL actions always require human intervention, while LOW, MEDIUM, and HIGH actions can be configured to auto-approve after a specific timeout using `register_action` rules.

**Q: Can I check if an action is still pending?**
Yes, you can use the `check_action_status` tool to retrieve the current status, whether human input is required, and the remaining timeout duration.

**Q: What happens if a human doesn't respond in time?**
If the timeout period defined in your auto-approval rules passes, the action status will transition to EXPIRED via the `refresh_gate_states` process.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/human-approval-gate-manager](https://vinkius.com/ai-agent-connect/human-approval-gate-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Human Approval Gate Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `human-approval-gate-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Human Approval Gate Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "human-approval-gate-manager": {
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
