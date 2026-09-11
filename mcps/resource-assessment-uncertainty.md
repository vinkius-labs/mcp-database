# Resource Assessment Uncertainty MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/resource-assessment-uncertainty)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [statistics](../categories/statistics.md)

Quantify geological uncertainty using probabilistic Monte Carlo simulations.

## Description
This MCP server provides advanced statistical tools for quantifying volumetric uncertainty in geological resource assessments. By applying Monte Carlo simulations to probabilistic input ranges, it transforms deterministic estimates into a range of possible outcomes. Use `calculate_resource_uncertainty` to determine P10, P50, and P90 resource estimates, or `analyze_sensitivity` to identify which parameters like porosity or thickness most impact your results. It is designed to help geologists and engineers account for measurement error and geological risk through rigorous statistical modeling.


## Available Tools (4)
- **analyze_sensitivity**: Identifies which input parameter has the greatest impact on the final resource uncertainty
- **calculate_resource_uncertainty**: Performs the primary probabilistic calculation to determine the range of possible resource volumes
- **compare_scenarios**: Compares two different sets of resource assumptions to evaluate how changing a specific geological model affects risk
- **validate_parameter_bounds**: Checks if provided probabilistic ranges are physically or geologically plausible within standard industry limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Resource Assessment Uncertainty** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the resource uncertainty for an area of 100-150 sq km, thickness of 10-20m, porosity of 0.15-0.25, and saturation of 0.6-0.8."

**🤖 AI Agent:**
> The simulation results show a P90 of 125,000 units, a P50 of 185,000 units, and a P10 of 240,000 units, with a mean of 182,500 units.

---

**👤 You:**
> "Which parameter is most influential in my resource model?"

**🤖 AI Agent:**
> Based on the sensitivity analysis, porosity is the top influencer, contributing to 65% of the total variance in the resource estimate.

---

**👤 You:**
> "Are my input parameters for porosity and saturation valid?"

**🤖 AI Agent:**
> Yes, the parameters are within valid geological bounds.


## ❓ FAQ

**Q: What are P10, P50, and P90 estimates?**
These are cumulative probability values. P90 is a conservative estimate (90% probability of being exceeded), P50 is the median, and P10 is an optimistic estimate (10% probability of being exceeded).

**Q: How can I check if my input ranges are realistic?**
You can use the `validate_parameter_bounds` tool to check if your area, thickness, porosity, and saturation ranges fall within physically and geologically plausible limits.

**Q: Can I compare two different geological models?**
Yes, the `compare_scenarios` tool allows you to evaluate how changes in assumptions affect risk by comparing the delta between P50 and P90 values.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/resource-assessment-uncertainty](https://vinkius.com/ai-agent-connect/resource-assessment-uncertainty)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Resource Assessment Uncertainty** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `resource-assessment-uncertainty` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Resource Assessment Uncertainty** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "resource-assessment-uncertainty": {
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
