# Passivation Potential Determination MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/passivation-potential-determination)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Extracts critical electrochemical parameters from polarization curves of active-passive metals.

## Description
This MCP server provides specialized tools for electrochemical analysis of active-passive metals. It allows AI agents to process polarization curve data to identify key corrosion resistance indicators. Using `analyze_passivation_peaks`, agents can find the primary passivation potential. The `calculate_flade_potential` tool identifies the transition from passive to active states, while `evaluate_passive_stability` measures current density within a specific range. Finally, `detect_pitting_breakdown` identifies the potential where protective films fail. This bridge enables precise electrochemical characterization within any MCP-compatible client like Cursor or Claude Desktop.


## Available Tools (4)
- **analyze_passivation_peaks**: Identifies the primary passivation point from a set of potential and current data
- **calculate_flade_potential**: Determines the potential at which passivity is lost
- **detect_pitting_breakdown**: Identifies the potential at which the passive film fails
- **evaluate_passive_stability**: Measures the current density during the stable passive state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Passivation Potential Determination** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the primary passivation potential for this dataset: [{"potential": 0.1, "currentDensity": 0.01}, {"potential": 0.2, "currentDensity": 0.05}, {"potential": 0.3, "currentDensity": 0.1}, {"potential": 0.4, "currentDensity": 0.02}]"

**🤖 AI Agent:**
> The primary passivation potential is 0.3 V with a peak current density of 0.1 A/cm².

---

**👤 You:**
> "What is the passive current density in the range between 0.4V and 0.6V for this data?"

**🤖 AI Agent:**
> The average passive current density in the specified range is 0.005 A/cm² with a stability index of 0.92.

---

**👤 You:**
> "Check for pitting breakdown in the passive window from 0.4 to 0.8V."

**🤖 AI Agent:**
> Pitting breakdown was detected at 0.75V with a breakdown severity of 4.5.


## ❓ FAQ

**Q: What kind of data is required for analysis?**
The tools require an array of data points, where each point contains a potential value and a corresponding current density value.

**Q: How can I find the Flade potential?**
You can use the `calculate_flade_potential` tool by providing the polarization data and a target current density threshold.

**Q: Can this tool detect pitting corrosion?**
Yes, the `detect_pitting_breakdown` tool is specifically designed to identify the potential at which the passive film fails and current density increases significantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/passivation-potential-determination](https://vinkius.com/ai-agent-connect/passivation-potential-determination)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Passivation Potential Determination** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `passivation-potential-determination` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Passivation Potential Determination** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "passivation-potential-determination": {
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
