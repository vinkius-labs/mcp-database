# Gas Lift Design Optimization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/gas-lift-design-optimization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Optimize gas lift systems by calculating valve spacing, injection depths, and production improvements.

## Description
This MCP server provides specialized engineering tools for gas lift optimization. It allows AI agents to calculate the precise `calculate_unloading_sequence` required to reach operating depths, identify the `optimize_injection_depth` to maximize pressure reduction, and predict the `estimate_production_increase` resulting from optimized gas injection. Additionally, it can `design_mandrel_configuration` to provide mechanical requirements for the tubing string assembly.


## Available Tools (4)
- **calculate_unloading_sequence**: Determines the required vertical spacing between gas lift valves to successfully unload the well
- **design_mandrel_configuration**: Provides the mechanical requirements for the mandrel and valve setup
- **estimate_production_increase**: Predicts the additional fluid volume produced as a result of the gas lift optimization
- **optimize_injection_depth**: Identifies the most effective depth to inject gas to maximize the reduction in bottomhole pressure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gas Lift Design Optimization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the valve spacing for a well with a productivity index of 2.5, tubing diameter of 3.5, casing diameter of 7.0, injection pressure of 1500, and initial fluid density of 0.45."

**🤖 AI Agent:**
> The unloading sequence requires 4 valves with spacings of [500, 450, 400, 350] meters, reaching a total unloading depth of 1700 meters.

---

**👤 You:**
> "What is the optimal injection depth if the available pressure is 2000, the fluid gradient is 0.4, and the bottomhole pressure is 5000?"

**🤖 AI Agent:**
> The optimal injection depth is 5000 meters with an estimated pressure at depth of 2000.

---

**👤 You:**
> "Estimate the production increase for a current rate of 1000 bpd, a productivity index of 1.5, and a pressure reduction of 500."

**🤖 AI Agent:**
> The new production rate is 1750 bpd, representing a 75% increase.


## ❓ FAQ

**Q: How does this tool help with well unloading?**
The `calculate_unloading_sequence` tool determines the vertical spacing between valves needed to displace heavy fluids with gas, ensuring a successful transition to operating conditions.

**Q: Can I predict production gains?**
Yes, by using `estimate_production_increase`, you can calculate the expected new production rate and the percentage increase based on the pressure reduction achieved.

**Q: Does it provide mechanical hardware requirements?**
Yes, the `design_mandrel_configuration` tool provides the total mandrel count, string length, and a list of required components for the tubing assembly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/gas-lift-design-optimization](https://vinkius.com/en/ai-agent-connect/gas-lift-design-optimization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gas Lift Design Optimization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gas-lift-design-optimization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gas Lift Design Optimization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gas-lift-design-optimization": {
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
