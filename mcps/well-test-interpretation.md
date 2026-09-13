# Well-Test Interpretation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/well-test-interpretation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Analyzes pressure transient data to characterize reservoir properties and wellbore performance.

## Description
This MCP server provides expert-level pressure transient analysis (PTA). It connects AI agents to specialized tools for interpreting pressure and flow rate data. Using `analyze_flow_regimes`, agents can identify radial, linear, or dual-porosity flow patterns. The `calculate_reservoir_parameters` tool determines permeability and skin factor, while `detect_wellbore_storage` and `identify_boundary_effects` help distinguish early-time wellbore effects from late-time reservoir boundaries.


## Available Tools (4)
- **analyze_flow_regimes**: Identifies flow patterns
- **calculate_reservoir_parameters**: Calculates reservoir properties
- **detect_wellbore_storage**: Detects wellbore storage effects
- **identify_boundary_effects**: Identifies boundary effects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Well-Test Interpretation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Identify the flow regimes in this pressure data."

**🤖 AI Agent:**
> The analysis shows a period of Wellbore Storage followed by a stable Radial Flow regime.

---

**👤 You:**
> "Calculate the reservoir permeability and skin factor."

**🤖 AI Agent:**
> The reservoir permeability is 150 mD and the skin factor is -2.5.

---

**👤 You:**
> "Are there any boundary effects present in the late-time data?"

**🤖 AI Agent:**
> Yes, a constant pressure boundary was detected at a distance of 200 feet.


## ❓ FAQ

**Q: What kind of data is required for analysis?**
You need to provide pressure and derivative data, along with fluid and reservoir properties like viscosity and porosity.

**Q: Can this tool detect dual-porosity reservoirs?**
Yes, the `analyze_flow_regimes` tool is designed to detect the characteristic signature of dual-porosity systems.

**Q: How are reservoir properties calculated?**
Properties like permeability and skin factor are calculated using the `calculate_reservoir_parameters` tool based on identified flow regimes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/well-test-interpretation](https://vinkius.com/en/ai-agent-connect/well-test-interpretation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Well-Test Interpretation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `well-test-interpretation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Well-Test Interpretation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "well-test-interpretation": {
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
