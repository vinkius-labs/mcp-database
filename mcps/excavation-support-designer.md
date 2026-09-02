# Excavation Support Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/excavation-support-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Designs temporary excavation support systems including stability and bracing.

## Description
This MCP server provides specialized engineering tools for designing temporary excavation support systems. It allows AI agents to determine the most appropriate support type using `analyze_support_feasibility`, calculate required embedment and wall movement with `calculate_wall_stability`, determine strut spacing via `design_lateral_bracing`, and evaluate performance through `simulate_staged_excavation`.


## Available Tools (4)
- **analyze_support_feasibility**: Determine the most appropriate support type for given site conditions
- **calculate_wall_stability**: Calculate required embedment depth and lateral wall movement
- **design_lateral_bracing**: Determine the spacing of struts needed to hold the wall in place
- **simulate_staged_excavation**: Evaluate support system performance through various stages of soil removal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Excavation Support Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What support type is best for a 5m excavation in sand with groundwater at 2m?"

**🤖 AI Agent:**
> For a 5m excavation in sand with groundwater at 2m, a Sheet Pile support is recommended due to the water presence.

---

**👤 You:**
> "Calculate the strut spacing for a 10m excavation using Soldier Piles with a 50kPa surcharge."

**🤖 AI Agent:**
> The required strut spacing for this configuration is 3.5 meters.

---

**👤 You:**
> "Will a 4m embedment depth be stable for a 6m excavation in clay?"

**🤖 AI Agent:**
> No, a 4m embedment depth is insufficient; the stability analysis indicates a higher embedment is required to maintain a positive safety factor.


## ❓ FAQ

**Q: How do I choose between Soldier Pile and Sheet Pile?**
You can use the `analyze_support_feasibility` tool to evaluate soil type and groundwater levels to determine the best support method.

**Q: Can I simulate the entire excavation process?**
Yes, the `simulate_staged_excavation` tool allows you to model the support system's performance across multiple stages of soil removal.

**Q: How is wall deflection calculated?**
Wall deflection is calculated using the `calculate_wall_stability` tool, which considers excavation depth, embedment, soil properties, and groundwater levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/excavation-support-designer](https://vinkius.com/ai-agent-connect/excavation-support-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Excavation Support Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `excavation-support-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Excavation Support Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "excavation-support-designer": {
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
