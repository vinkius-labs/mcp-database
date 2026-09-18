# Child Growth Percentile Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/child-growth-percentile-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculate pediatric growth percentiles, velocity, and status using WHO and CDC standards.

## Description
This MCP server provides clinical-grade pediatric growth analysis. It connects AI agents to standardized WHO and CDC growth reference data to monitor child development. Using tools like `get_growth_percentiles`, agents can determine height, weight, and BMI percentiles. The `get_growth_velocity` tool tracks how measurements change over time, while `get_growth_status` evaluates if a child's growth falls within normal clinical ranges. It also supports prematurity adjustments for accurate infant monitoring.


## Available Tools (4)
- **get_growth_percentiles**: Calculates current percentile rankings for a child's physical measurements
- **get_growth_status**: Evaluates whether a child's growth is within a clinically normal range
- **get_growth_velocity**: Determines how quickly a child's measurements have changed between two time points
- **validate_measurement_integrity**: Checks if the provided physical measurements are biologically plausible


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Child Growth Percentile Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the growth percentile for a 12-month-old male, 75cm tall and 9kg?"

**🤖 AI Agent:**
> The 12-month-old male has a height percentile of 25th, a weight percentile of 15th, and a BMI percentile of 20th.

---

**👤 You:**
> "Calculate the growth velocity for a girl who was 60cm at 6 months and 64cm at 9 months."

**🤖 AI Agent:**
> The height velocity is 1.33 cm per month.

---

**👤 You:**
> "Is a child with a 90th percentile weight status considered high?"

**🤖 AI Agent:**
> Yes, a percentile above the 85th percentile is classified as a high status.


## ❓ FAQ

**Q: Which growth standards are used?**
The server uses WHO standards for children aged 0-24 months and CDC growth charts for children aged 2-20 years.

**Q: How does the tool handle premature infants?**
When `isPremature` is enabled, the `get_growth_percentiles` tool calculates a corrected age based on gestational weeks to ensure accurate percentile comparison.

**Q: Can I check if a child's growth is normal?**
Yes, you can use the `get_growth_status` tool to evaluate if percentiles fall within the clinically normal range (5th to 85th percentile).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/child-growth-percentile-calculator](https://vinkius.com/en/ai-agent-connect/child-growth-percentile-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Child Growth Percentile Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `child-growth-percentile-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Child Growth Percentile Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "child-growth-percentile-calculator": {
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
