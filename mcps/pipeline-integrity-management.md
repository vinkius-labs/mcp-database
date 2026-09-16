# Pipeline Integrity Management MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pipeline-integrity-management)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Plan and manage pipeline integrity programs using risk-based methodologies.

## Description
This MCP server provides a specialized system for planning and managing pipeline integrity programs. It uses the Pipeline Integrity Management System (PIMS) framework to identify and mitigate threats. Users can evaluate segment risks with `get_risk_profile`, determine inspection frequencies using `calculate_inspection_schedule`, prioritize repairs via `generate_maintenance_plan`, and verify legal standing with `evaluate_regulatory_compliance`. It is designed to handle High Consequence Areas (HCA) and various inspection methods like ILI and Direct Assessment.


## Available Tools (4)
- **calculate_inspection_schedule**: Determines the required frequency for future inspections
- **evaluate_regulatory_compliance**: Checks if the current integrity program meets legal and standard mandates
- **generate_maintenance_plan**: Ranks and lists pipeline segments that require immediate attention
- **get_risk_profile**: Evaluates the current risk level of a specific pipeline segment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pipeline Integrity Management** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the risk profile for segment ID 5502?"

**🤖 AI Agent:**
> The risk score for segment 5502 is 75, it is located in a High Consequence Area, and the primary threats identified are corrosion and external interference.

---

**👤 You:**
> "When is the next ILI inspection due for segment 1024?"

**🤖 AI Agent:**
> The next ILI inspection for segment 1024 is due on 2025-06-15, with a recommended interval of 24 months.

---

**👤 You:**
> "Show me critical maintenance items that need attention."

**🤖 AI Agent:**
> The following segments require critical maintenance: Segment 882 (Priority: 92, Action: Immediate Pressure Test) and Segment 415 (Priority: 88, Action: Repair coating degradation).


## ❓ FAQ

**Q: How do I check if a pipeline segment is in a High Consequence Area?**
You can use the `get_risk_profile` tool. It returns an `isHca` boolean indicating if the segment is located within a High Consequence Area.

**Q: Can I schedule inspections for specific methods like ILI?**
Yes, the `calculate_inspection_schedule` tool allows you to specify the `inspectionMethod`, including ILI, DA, or Pressure Testing.

**Q: How are maintenance tasks prioritized?**
Maintenance tasks are ranked using `generate_maintenance_plan`, which calculates priority based on risk scores, segment age, and time since the last inspection.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pipeline-integrity-management](https://vinkius.com/en/ai-agent-connect/pipeline-integrity-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pipeline Integrity Management** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pipeline-integrity-management` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pipeline Integrity Management** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pipeline-integrity-management": {
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
