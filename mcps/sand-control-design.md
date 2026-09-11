# Sand Control Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sand-control-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design sand control methods for unconsolidated formations.

## Description
This MCP server provides specialized engineering tools for designing sand control systems in unconsolidated geological formations. It enables precise calculations for `analyze_formation_stability` to assess sand production risk, `calculate_gravel_pack_size` for optimal gravel selection, `determine_screen_slot_width` for mechanical filter sizing, and `evaluate_plugging_risk` to predict fines migration impacts. It bridges the gap between geological grain size distribution data and practical wellbore completion hardware.


## Available Tools (4)
- **analyze_formation_stability**: Assesses the risk of sand production based on formation strength and grain properties
- **evaluate_plugging_risk**: Predicts the likelihood of the sand control system becoming blocked by fine particles
- **calculate_gravel_pack_size**: Determines the optimal diameter of gravel to be used in a gravel pack completion
- **determine_screen_slot_width**: Calculates the physical opening width required for the mechanical screen


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sand Control Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the sand production risk for a formation with strength 500 and a drawdown of 200?"

**🤖 AI Agent:**
> The sand production risk is rated as Low with a stability rating of Stable.

---

**👤 You:**
> "Calculate the gravel pack size using the Saucier method for this distribution: [{"size": 0.1, "percent": 100}]"

**🤖 AI Agent:**
> The optimal gravel size is 0.15 units with a retention ratio of 1.5.

---

**👤 You:**
> "What slot width do I need for a 0.25 gravel size filtering the gravel?"

**🤖 AI Agent:**
> The required slot width is 0.20 units.


## ❓ FAQ

**Q: How do I assess if my formation is stable?**
You can use the `analyze_formation_stability` tool by providing the grain size distribution, formation strength, and expected production pressure.

**Q: Can this tool help select gravel sizes?**
Yes, the `calculate_gravel_pack_size` tool determines the optimal gravel diameter based on your formation's grain size distribution and chosen design method.

**Q: How is plugging risk evaluated?**
The `evaluate_plugging_risk` tool predicts the likelihood of blockage by analyzing grain size distribution, flow rate, and slot width.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sand-control-design](https://vinkius.com/en/ai-agent-connect/sand-control-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sand Control Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sand-control-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sand Control Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sand-control-design": {
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
