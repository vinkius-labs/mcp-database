# PPE Requirements Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ppe-requirements-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [risk-assessment](../categories/risk-assessment.md)

Determines mandatory Personal Protective Equipment based on work activities and hazards.

## Description
This MCP server provides a decision-support system for safety professionals and operators. It calculates required PPE across categories like head, eye, hand, foot, and body protection by analyzing specific work activities, identified hazards, and exposure intensities. Use `evaluate_ppe_needs` to determine specific equipment, `check_ppe_compatibility` to ensure selected items work together, `get_hazard_severity_index` to quantify risk, and `get_task_risk_profile` to understand baseline hazards for any task.


## Available Tools (4)
- **get_task_risk_profile**: Provides a summary of the risk landscape for a specific work activity
- **check_ppe_compatibility**: Validates if a set of selected PPE items can be worn together
- **evaluate_ppe_needs**: Determines the specific PPE requirements for a given set of task parameters
- **get_hazard_severity_index**: Calculates a standardized severity score based on hazards and intensities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PPE Requirements Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What PPE is required for welding with high heat and light exposure?"

**🤖 AI Agent:**
> For welding with high heat and light exposure, you require welding helmet, heat-resistant gloves, and flame-retardant coveralls.

---

**👤 You:**
> "Are safety goggles and a full-face respirator compatible?"

**🤖 AI Agent:**
> No, the full-face respirator may interfere with the seal and fit of standard safety goggles.

---

**👤 You:**
> "What are the typical hazards for chemical mixing?"

**🤖 AI Agent:**
> Typical hazards for chemical mixing include chemical splashes, vapor inhalation, and skin irritation.


## ❓ FAQ

**Q: How do I determine what PPE is needed for a new task?**
You can use the `evaluate_ppe_needs` tool by providing the work activity, the list of hazards, and the intensity of those hazards.

**Q: Can I check if my selected safety gear is safe to wear together?**
Yes, the `check_ppe_compatibility` tool validates if your selected items might conflict with each other.

**Q: How is the risk level calculated?**
The `get_hazard_severity_index` tool calculates a standardized score based on the combination of hazard types and their exposure levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ppe-requirements-assessment](https://vinkius.com/en/ai-agent-connect/ppe-requirements-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PPE Requirements Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ppe-requirements-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PPE Requirements Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ppe-requirements-assessment": {
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
