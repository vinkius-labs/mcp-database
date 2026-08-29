# Quality Control Chart Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/quality-control-chart-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [statistics](../categories/statistics.md)

Designs statistical process control charts to monitor process stability.

## Description
This MCP server provides essential tools for Statistical Process Control (SPC). It allows AI agents to calculate control limits, identify center lines, and detect out-of-control patterns in manufacturing or service processes. Using tools like `calculate_control_parameters` and `analyze_process_stability`, agents can determine if a process is stable or if it exhibits non-random trends and shifts.


## Available Tools (4)
- **generate_individual_limits**: Specifically calculates limits for processes where measurements are taken one at a time (Individual charts)
- **analyze_process_stability**: Determines if a process is in a state of statistical control based on provided measurements and chart type
- **calculate_control_parameters**: Generates the mathematical boundaries for a specific SPC chart type
- **detect_out_of_control_patterns**: Identifies specific non-random patterns in a sequence of data points


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Quality Control Chart Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the control limits for these subgroups: [[10, 12], [11, 13], [9, 11]] using an x_bar chart."

**🤖 AI Agent:**
> The calculated parameters for the x_bar chart are: UCL: 13.5, LCL: 8.5, and Center Line: 11.0.

---

**👤 You:**
> "Is this process stable? Measurements: [10, 10, 10, 15, 10], chartType: 'individual', controlLimits: {"ucl": 12, "lcl": 8}, centerLine: 10"

**🤖 AI Agent:**
> The process is unstable. A violation was detected because the measurement 15 falls outside the upper control limit of 12.

---

**👤 You:**
> "Find patterns in this series: [10, 11, 12, 13, 14, 15], centerLine: 10, ucl: 20, lcl: 0"

**🤖 AI Agent:**
> A trend pattern was detected in the series.


## ❓ FAQ

**Q: What types of charts can I design?**
You can design X-bar, R, S, and Individual (I) charts using the `calculate_control_parameters` and `generate_individual_limits` tools.

**Q: How do I check if my process is stable?**
Use the `analyze_process_stability` tool with your measurements and control limits to detect violations and stability status.

**Q: Can I detect trends in my data?**
Yes, the `detect_out_of_control_patterns` tool is specifically designed to identify trends, shifts, and oscillations in your data series.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/quality-control-chart-design](https://vinkius.com/ai-agent-connect/quality-control-chart-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Quality Control Chart Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `quality-control-chart-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Quality Control Chart Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "quality-control-chart-design": {
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
