# Cut-Off Grade Optimization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/cut-off-grade-optimization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Optimize mining cut-off grades to maximize NPV and production efficiency.

## Description
This MCP server provides specialized tools for mining engineers and financial analysts to optimize ore classification. By using `optimize_cut_off_grade`, users can identify the specific grade that maximizes Net Present Value (NPV) while accounting for opportunity costs. The server also includes `calculate_break_even_grade` to determine minimum profitable thresholds, `simulate_production_schedule` to project annual cash flows and mine life, and `evaluate_stockpile_viability` to decide if low-grade material should be stockpiled or discarded. It serves as a bridge between complex mining economic models and AI agents.


## Available Tools (4)
- **calculate_break_even_grade**: Determines the minimum grade required to cover all incremental costs of processing
- **evaluate_stockpile_viability**: Determines if diverted low-grade material should be stockpiled or sent to waste
- **optimize_cut_off_grade**: Identifies the specific grade that maximizes the Net Present Value of the operation
- **simulate_production_schedule**: Projects the sequence of mining and processing activities over time based on a chosen grade


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cut-Off Grade Optimization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the optimal cut-off grade for a gold mine with a metal price of 2000, recovery of 0.9, mining cost of 50, processing cost of 30, dilution of 0.05, and opportunity cost of 10?"

**🤖 AI Agent:**
> The optimal cut-off grade for this operation is 0.15.

---

**👤 You:**
> "Calculate the break-even grade if the metal price is 1500, recovery is 0.85, mining cost is 40, processing cost is 25, and dilution is 0.1?"

**🤖 AI Agent:**
> The break-even grade is 0.12.

---

**👤 You:**
> "Should I stockpile material with a grade of 0.05 if the metal price is 1800, recovery is 0.8, processing cost is 20, storage cost is 2, and dilution is 0.05?"

**🤖 AI Agent:**
> The action is stockpile.


## ❓ FAQ

**Q: How does this tool help maximize NPV?**
It uses `optimize_cut_off_grade` to find the ideal balance between immediate high-grade production and long-term mine value, accounting for opportunity costs.

**Q: Can I simulate my mine's production over time?**
Yes, the `simulate_production_schedule` tool allows you to project annual ore tonnage, metal production, and cash flow based on your chosen cut-off grade.

**Q: What is the difference between break-even and optimal grade?**
The break-even grade, found via `calculate_break_even_grade`, is the minimum to cover costs. The optimal grade is typically higher as it accounts for the opportunity cost of delaying future cash flows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/cut-off-grade-optimization](https://vinkius.com/ai-agent-connect/cut-off-grade-optimization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cut-Off Grade Optimization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cut-off-grade-optimization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cut-Off Grade Optimization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cut-off-grade-optimization": {
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
