# Tree Well Danger Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tree-well-danger-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [risk-assessment](../categories/risk-assessment.md)

Calculates tree well suffocation risk and escape feasibility.

## Description
This MCP server provides critical safety assessments for backcountry riders. It uses environmental data to calculate suffocation risk, evaluate how difficult it is to climb out of a snow cavity, and assess the viability of rescue operations. By using `calculate_risk_profile`, users can determine the immediate danger level, while `evaluate_escape_feasibility` helps predict physical escape success. It also includes `assess_rescue_viability` to check if available gear and partner proximity are sufficient for a successful rescue.


## Available Tools (4)
- **assess_rescue_viability**: Evaluates the likelihood of a successful rescue based on partner presence and gear
- **calculate_risk_profile**: Provides a high-level summary of the danger level and immediate survival prognosis
- **evaluate_escape_feasibility**: Determines if a rider can realistically climb out of the well based on the physical environment
- **get_safety_guidelines**: Provides customized safety protocols based on specific environmental and situational factors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tree Well Danger Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the risk if I fall face down in 200cm of snow with a 1m wide well?"

**🤖 AI Agent:**
> The risk score is 9/10. The primary danger is Asphyxiation due to the face-down orientation and high snow depth.

---

**👤 You:**
> "Can I get out of a 150cm deep well with a 2m diameter?"

**🤖 AI Agent:**
> The escape success probability is 0.7 with moderate physical effort required.

---

**👤 You:**
> "Is my rescue viable if my partner is 10m away with a shovel?"

**🤖 AI Agent:**
> The rescue window status is Optimal with a survival probability of 0.9.


## ❓ FAQ

**Q: How accurate is the risk score?**
The risk score provided by `calculate_risk_profile` is a mathematical model based on snow depth, tree type, and rider orientation to estimate danger levels.

**Q: Can I use this to plan a rescue?**
You can use `assess_rescue_viability` to evaluate if your current equipment and partner proximity are sufficient for a rescue scenario.

**Q: What factors influence escape difficulty?**
The `evaluate_escape_feasibility` tool considers snow depth, well diameter, and tree type to determine how hard it is to climb out.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tree-well-danger-assessment](https://vinkius.com/en/ai-agent-connect/tree-well-danger-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tree Well Danger Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tree-well-danger-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tree Well Danger Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tree-well-danger-assessment": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
