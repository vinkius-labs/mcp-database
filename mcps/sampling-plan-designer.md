# Sampling Plan Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sampling-plan-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [statistics](../categories/statistics.md)

Generates statistically rigorous sampling plans for quality control.

## Description
This MCP server provides tools to design and evaluate statistical sampling plans for analytical quality control. It allows users to calculate fundamental parameters like sample size and acceptance numbers, retrieve standardized plans from ISO 2859 or ANSI/ASQ, generate Operating Characteristic (OC) curves, and compare different plans to determine which is more conservative for a given defect rate. Use `calculate_basic_plan` to find optimal parameters, `lookup_standard_plan` for industry standards, and `get_oc_curve_data` for visualization data.


## Available Tools (4)
- **calculate_basic_plan**: Generates the fundamental parameters of a sampling plan (n and c) based on target quality and risk levels
- **compare_plans**: Evaluates two different sampling plans to determine which is more stringent or carries less risk
- **get_oc_curve_data**: Provides a series of data points to plot the Operating Characteristic curve for a specific plan
- **lookup_standard_plan**: Retrieves a pre-defined sampling plan from ISO 2859 or ANSI/ASQ tables based on lot size and inspection level


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sampling Plan Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a sampling plan for a lot of 5000 units with an AQL of 0.01, producer risk of 0.05, and consumer risk of 0.10."

**🤖 AI Agent:**
> For a lot size of 5000 with an AQL of 1%, the calculated sample size is 132 and the acceptance number is 3.

---

**👤 You:**
> "What is the standard plan for a lot size of 1000 using ISO 2859 General II inspection?"

**🤖 AI Agent:**
> The ISO 2859 General II plan for a lot size of 1000 specifies a sample size of 80 and an acceptance number of 2.

---

**👤 You:**
> "Compare a plan with sample size 50 and acceptance number 1 against a plan with sample size 80 and acceptance number 2 at a 2% defect rate."

**🤖 AI Agent:**
> At a 2% defect rate, the plan with sample size 80 and acceptance number 2 is more conservative.


## ❓ FAQ

**Q: How do I generate a plan based on specific risk levels?**
You can use the `calculate_basic_plan` tool by providing the lot size, target AQL, producer risk, and consumer risk.

**Q: Can I use industry standards like ISO 2859?**
Yes, the `lookup_standard_plan` tool allows you to retrieve plans directly from ISO 2859 and ANSI/ASQ tables.

**Q: How can I compare two different sampling plans?**
Use the `compare_plans` tool to evaluate two plans against a specific defect rate to see which is more stringent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sampling-plan-designer](https://vinkius.com/ai-agent-connect/sampling-plan-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sampling Plan Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sampling-plan-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sampling Plan Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sampling-plan-designer": {
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
