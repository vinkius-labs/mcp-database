# Smart Pig Inspection Planning MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/smart-pig-inspection-planning)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [predictive-maintenance](../categories/predictive-maintenance.md)

Optimize pipeline inspection programs using degradation physics and historical data.

## Description
This MCP server provides intelligent decision support for pipeline operators. It uses degradation models to calculate optimal inspection intervals, determine necessary tool requirements like MFL or UT, and predict expected findings. Operators can assess risk levels to ensure pipeline integrity through data-driven planning.


## Available Tools (4)
- **determine_tool_requirements**: Identifies which tool types and sensitivity levels are necessary for a specific pipeline segment
- **evaluate_inspection_risk**: Assesses the risk profile of the current inspection plan
- **plan_inspection_interval**: Determines the optimal time until the next inspection is required
- **predict_inspection_findings**: Forecasts the types and quantities of defects likely to be found in the next inspection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Smart Pig Inspection Planning** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "When should we next inspect pipeline P-101 if the degradation rate is 0.05 and the threshold is 2.0?"

**🤖 AI Agent:**
> The next inspection for pipeline P-101 is scheduled for 2026-05-15 with a confidence level of 0.92.

---

**👤 You:**
> "What tool do I need to detect corrosion in pipeline P-202?"

**🤖 AI Agent:**
> For corrosion detection in pipeline P-202, an MFL tool is recommended with a minimum resolution of 0.5.

---

**👤 You:**
> "What is the risk level for a 5-year interval on pipeline P-303?"

**🤖 AI Agent:**
> The risk score for a 5-year interval on pipeline P-303 is 0.75, which is classified as High risk.


## ❓ FAQ

**Q: How is the next inspection date calculated?**
The `plan_inspection_interval` tool calculates the date by modeling the time it takes for a detected flaw to reach a critical threshold based on the current degradation rate.

**Q: Can I determine which tool to use for corrosion?**
Yes, using `determine_tool_requirements` with a target flaw type of 'corrosion' will recommend appropriate tools like MFL or UT.

**Q: How accurate are the predicted findings?**
The `predict_inspection_findings` tool generates forecasts by projecting historical flaw data forward using established degradation models.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/smart-pig-inspection-planning](https://vinkius.com/en/ai-agent-connect/smart-pig-inspection-planning)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Smart Pig Inspection Planning** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `smart-pig-inspection-planning` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Smart Pig Inspection Planning** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "smart-pig-inspection-planning": {
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
