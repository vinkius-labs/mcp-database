# Agent Config Drift Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-config-drift-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Detects unauthorized changes to agent configurations by comparing SHA-256 hashes.

## Description
This MCP server ensures the integrity of LLM agent configurations by detecting 'drift'--unintended or unauthorized modifications to critical parameters. It uses deterministic SHA-256 hashing to compare current configurations against a known good baseline. By monitoring fields like system prompts and permissions, it identifies specific deviations and calculates a risk severity score. Use `check_config_integrity` to detect changes, `get_drift_report` for granular diffs, and `evaluate_risk_level` to assess the impact of detected drift.


## Available Tools (3)
- **check_config_integrity**: Determines if the current agent configuration has deviated from its authorized baseline
- **evaluate_risk_level**: Calculates the severity of a detected drift based on the nature of the changes
- **get_drift_report**: Provides a detailed breakdown of the specific differences between two versions of a configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Config Drift Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if the current configuration for agent 'auth-service-01' has drifted."

**🤖 AI Agent:**
> {"hasDrifted": true, "currentHash": "a1b2c3d4...", "driftSeverity": "HIGH", "changedFields": [{"field": "system_prompt", "oldVal": "...", "newVal": "..."}]}

---

**👤 You:**
> "What is the risk level for these changed fields: ['permissions', 'allowed_tools']?"

**🤖 AI Agent:**
> {"severity": "CRITICAL", "riskScore": 95}

---

**👤 You:**
> "Get a detailed drift report for agent 'data-processor' between version v1.0 and v1.1."

**🤖 AI Agent:**
> {"fieldName": "allowed_tools", "type": "addition", "oldValue": "["read_db"]", "newValue": "["read_db", "write_db"]", "severityImpact": "LOW"}


## ❓ FAQ

**Q: How does the drift detection work?**
The server computes a deterministic SHA-256 hash of critical configuration sections and compares it against a stored baseline. If the hashes differ, it performs a deep inspection to find the exact changed fields.

**Q: What is considered a high-severity drift?**
Changes to 'permissions' are considered the highest risk, followed by modifications to the 'system_prompt'.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, this MCP server can be connected to Cursor, Claude Desktop, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-config-drift-detector](https://vinkius.com/ai-agent-connect/agent-config-drift-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Config Drift Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-config-drift-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Config Drift Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-config-drift-detector": {
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
