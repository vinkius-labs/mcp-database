# Wine Tasting Panel Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-tasting-panel-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [quality-control](../categories/quality-control.md)

Design sensory tasting panels for wine quality control by calculating panelist requirements and reliability.

## Description
This MCP server provides tools to design sensory tasting panels for wine quality control. It calculates the necessary number of panelists and replications based on test types like difference, descriptive, or preference testing. Use `calculate_panel_requirements` to determine headcount, `select_qualified_panelists` to filter candidates based on sensitivity and consistency, `evaluate_panel_performance` to analyze historical data, and `predict_test_reliability` to estimate the success probability of a designed panel.


## Available Tools (4)
- **calculate_panel_requirements**: Determines the minimum number of panelists and replications needed for a specific sensory test
- **evaluate_panel_performance**: Analyzes historical or current tasting data to assess the reliability of the panel
- **predict_test_reliability**: Estimates the likelihood that the designed panel will successfully meet its objectives before the test begins
- **select_qualified_panelists**: Filters a list of available panelists to find those who meet the specific requirements of a designed test


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Tasting Panel Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many panelists and replications do I need for a difference test with 0.95 statistical power, 0.8 sensitivity, and 0.7 consistency?"

**🤖 AI Agent:**
> For a difference test with those parameters, you will need 12 panelists with 3 replications each, totaling 36 tastings.

---

**👤 You:**
> "I have a list of panelists. Can you find 5 people who have at least 0.8 sensitivity and 0.8 consistency?"

**🤖 AI Agent:**
> The following 5 panelists have been selected: Panelist ID 102, 105, 110, 115, and 120.

---

**👤 You:**
> "What is the average consistency of my panel based on these tasting records?"

**🤖 AI Agent:**
> The average consistency for the provided tasting records is 0.78.


## ❓ FAQ

**Q: How do I determine how many people I need for a descriptive test?**
You can use the `calculate_panel_requirements` tool by providing the test type as 'descriptive', your desired statistical power, and the expected sensitivity and consistency of your panel.

**Q: Can I filter panelists by their specific scores?**
Yes, the `select_qualified_panelists` tool allows you to filter available candidates using minimum sensitivity and consistency thresholds.

**Q: How can I check if my panel is reliable enough for a new test?**
Use the `predict_test_reliability` tool. It takes your design parameters and current panel performance to provide a reliability score and risk level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-tasting-panel-design](https://vinkius.com/en/ai-agent-connect/wine-tasting-panel-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Tasting Panel Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-tasting-panel-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Tasting Panel Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-tasting-panel-design": {
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
