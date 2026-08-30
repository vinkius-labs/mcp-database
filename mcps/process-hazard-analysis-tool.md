# Process Hazard Analysis Tool MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/process-hazard-analysis-tool)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Systematic documentation and risk assessment for industrial process hazards.

## Description
This MCP server provides a structured framework for conducting Process Hazard Analysis (PHA). It allows users to document hazards using methodologies like HAZOP, What-If, or Checklist. Users can use `create_hazard_entry` to record deviations, `add_safeguard` to link safety controls, and `evaluate_risk_level` to determine residual risk. The tool also supports `generate_recommendations` to create mitigation strategies and `list_process_summary` for high-level risk profiling.


## Available Tools (5)
- **add_safeguard**: Associate an existing safety control with a specific hazard
- **create_hazard_entry**: Record a new identified hazard within a specific process description
- **evaluate_risk_level**: Recalculate or view the current risk ranking of a hazard
- **generate_recommendations**: Produce required safety improvements and follow-up tasks
- **list_process_summary**: Provide a high-level overview of all hazards identified within a specific process


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Process Hazard Analysis Tool** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Record a new hazard for a chemical reactor where temperature exceeds 500C using HAZOP."

**🤖 AI Agent:**
> Hazard entry created: Temperature deviation in chemical reactor recorded with high consequence.

---

**👤 You:**
> "Add a pressure relief valve as a safeguard for the reactor hazard."

**🤖 AI Agent:**
> Safeguard 'Pressure Relief Valve' successfully added to the hazard.

---

**👤 You:**
> "What is the current risk summary for the chemical reactor process?"

**🤖 AI Agent:**
> The process summary shows 3 total hazards, with 1 high-risk hazard identified.


## ❓ FAQ

**Q: What methodologies are supported?**
The tool supports HAZOP, What-If, and Checklist methodologies for hazard identification.

**Q: How is risk calculated?**
Risk is determined by combining the likelihood and consequence severity, which can be updated using `evaluate_risk_level` after adding safeguards.

**Q: Can I generate action items?**
Yes, by using `generate_recommendations`, the tool produces specific action items to implement mitigation strategies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/process-hazard-analysis-tool](https://vinkius.com/ai-agent-connect/process-hazard-analysis-tool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Process Hazard Analysis Tool** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `process-hazard-analysis-tool` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Process Hazard Analysis Tool** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "process-hazard-analysis-tool": {
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
