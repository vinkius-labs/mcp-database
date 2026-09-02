# Process Safety Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/process-safety-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [risk-management](../categories/risk-management.md)

Conduct HAZOP, LOPA, and SIL assessments to manage industrial process risks.

## Description
This MCP server provides a specialized toolset for quantitative and qualitative process safety assessments. It enables AI agents to perform Hazard and Operability (HAZOP) studies using `analyze_hazop_nodes`, conduct Layer of Protection Analysis (LOPA) via `calculate_lopa_risk`, and determine necessary Safety Integrity Levels (SIL) with `determine_sil_requirement`. Users can also access standardized safety data through `query_safety_catalog` to ensure compliance with industry safety standards.


## Available Tools (4)
- **analyze_hazop_nodes**: g., No, More, Less), and process parameters (e.g., Flow, Pressure).

Identify potential deviations in a process node based on guide words and parameters
- **calculate_lopa_risk**: Determine the residual risk of a scenario after accounting for all protection layers
- **determine_sil_requirement**: Calculate the required Safety Integrity Level (SIL) for a safety function
- **query_safety_catalog**: Retrieve predefined hazard profiles or safeguard standards


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Process Safety Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Perform a HAZOP analysis for the 'Reactor Feed Line' node using 'No' and 'More' as guide words for 'Flow'."

**🤖 AI Agent:**
> The HAZOP analysis for Reactor Feed Line identified two deviations: 1. No Flow (Cause: Valve failure, Consequence: Reactor starvation, Safeguard: Low flow alarm) and 2. More Flow (Cause: Control valve failure, Consequence: Overfilling, Safeguard: High level switch).

---

**👤 You:**
> "Calculate the residual risk for a scenario with an initiating event frequency of 0.1 and two protection layers with PFDs of 0.1 and 0.01."

**🤖 AI Agent:**
> The frequency of consequence is 0.0001 per year.

---

**👤 You:**
> "What SIL is required if the target risk reduction is 100 and current mitigation is 10?"

**🤖 AI Agent:**
> The required SIL is SIL 1.


## ❓ FAQ

**Q: What methodologies are supported?**
The server supports HAZOP, LOPA, and SIL requirement calculations.

**Q: How do I perform a HAZOP study?**
You can use the `analyze_hazop_nodes` tool by providing the node name, guide words, and process parameters.

**Q: Can I access safety standards?**
Yes, the `query_safety_catalog` tool allows you to retrieve predefined hazard profiles and safeguard standards.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/process-safety-analysis](https://vinkius.com/ai-agent-connect/process-safety-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Process Safety Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `process-safety-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Process Safety Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "process-safety-analysis": {
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
