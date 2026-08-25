# Accelerator Graduation Metrics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-graduation-metrics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Calculates program completion, attrition, and graduation time metrics for accelerator cohorts.

## Description
This MCP server provides deep insights into accelerator program performance. It allows AI agents to analyze cohort success by calculating graduation rates, drop rates, and time-to-graduation distributions. Using tools like `get_graduation_metrics`, `get_completion_time_distribution`, and `analyze_attrition_drivers`, agents can identify why companies exit programs and how program intensity affects outcomes.


## Available Tools (3)
- **analyze_attrition_drivers**: Analyze the primary reasons for company attrition in a specific cohort
- **get_completion_time_distribution**: Get the distribution of completion times for a specific cohort
- **get_graduation_metrics**: Get high-level success and attrition percentages for a specific cohort


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Graduation Metrics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the graduation rate for cohort C2023?"

**🤖 AI Agent:**
> The graduation rate for cohort C2023 is 85%, with a drop rate of 15%.

---

**👤 You:**
> "How long does it take for companies in cohort C2023 to graduate?"

**🤖 AI Agent:**
> The average completion time for cohort C2023 is 6 months, with a median of 5.5 months.

---

**👤 You:**
> "Why are companies dropping out of cohort C2023?"

**🤖 AI Agent:**
> The primary reason for attrition in cohort C2023 is poor selection fit, with a correlation score of 0.75.


## ❓ FAQ

**Q: What metrics can I track?**
You can track graduation rates, drop rates, average completion times, and primary drivers of attrition using the available tools.

**Q: How does program intensity affect the data?**
The `get_graduation_metrics` tool allows you to specify an intensity level, which helps in determining if attrition is within healthy thresholds for that specific rigor.

**Q: Can I analyze why companies are dropping out?**
Yes, the `analyze_attrition_drivers` tool provides the primary reason for drops and can correlate these with selection fit scores.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-graduation-metrics](https://vinkius.com/ai-agent-connect/accelerator-graduation-metrics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Graduation Metrics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-graduation-metrics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Graduation Metrics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-graduation-metrics": {
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
