# Wellbore Cleaning Efficiency MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wellbore-cleaning-efficiency)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Evaluates hole cleaning effectiveness and cuttings transport efficiency.

## Description
This MCP server provides analytical tools to evaluate the effectiveness of cuttings transport and the accumulation of cuttings beds during drilling operations. It allows AI agents to calculate `bed_height`, determine `critical_velocity`, and `optimize_flow_rate` based on mud rheology, hole angle, and ROP. Use `evaluate_cleaning_risk` to receive safety assessments and recommendations to prevent stuck pipe and pressure issues.


## Available Tools (4)
- **calculate_bed_height**: Determines the thickness of the cuttings bed accumulated at a specific section of the wellbore
- **determine_critical_velocity**: Calculates the minimum fluid velocity required to prevent or remove a cuttings bed
- **evaluate_cleaning_risk**: Provides a high-level safety assessment based on current drilling parameters
- **optimize_flow_rate**: Recommends the necessary flow rate to achieve a target cleaning efficiency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wellbore Cleaning Efficiency** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected bed height for a 45 degree hole with a viscosity of 20, flow rate of 500, ROP of 15, and cuttings size of 0.005?"

**🤖 AI Agent:**
> The calculated bed height is 0.025 meters with a cleaning efficiency of 85% and a Low risk level.

---

**👤 You:**
> "Calculate the minimum velocity needed for a 60 degree well with a mud yield point of 15, cuttings size of 0.008, and fluid density of 1100."

**🤖 AI Agent:**
> The critical velocity required is 0.45 m/s with a safety threshold of 0.52 m/s.

---

**👤 You:**
> "I have a bed height of 0.15m in a 12.25 inch hole at a 75 degree angle. What is the risk?"

**🤖 AI Agent:**
> The risk score is 75, which is a Warning level. It is recommended to increase flow rate or circulate bottoms up.


## ❓ FAQ

**Q: How can I check if my wellbore is at risk of stuck pipe?**
You can use the `evaluate_cleaning_risk` tool to get a risk score and alert level based on your current bed height and wellbore diameter.

**Q: What parameters are needed to calculate the required flow rate?**
To use `optimize_flow_rate`, you need to provide the target efficiency, hole angle, mud viscosity, ROP, and cuttings size.

**Q: Does this tool account for hole inclination?**
Yes, all core tools like `calculate_bed_height` and `determine_critical_velocity` require the hole angle to account for gravity-driven cuttings settling in inclined wells.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wellbore-cleaning-efficiency](https://vinkius.com/en/ai-agent-connect/wellbore-cleaning-efficiency)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wellbore Cleaning Efficiency** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wellbore-cleaning-efficiency` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wellbore Cleaning Efficiency** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wellbore-cleaning-efficiency": {
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
