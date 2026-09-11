# E&P Portfolio Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ep-portfolio-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Optimize energy project portfolios by balancing returns, risk, and capital constraints.

## Description
This MCP server provides advanced tools for Exploration & Production (E&P) portfolio management. It allows AI agents to evaluate project inventories using `analyze_project_inventory_tool`, determine the most efficient project combinations with `calculate_optimal_mix_tool`, and stress-test selections via `simulate_risk_scenarios_tool`. Additionally, it ensures corporate goals are met through `evaluate_strategic_alignment_tool`. It is designed to help energy companies maximize value while managing volatility and budget limits.


## Available Tools (4)
- **calculate_optimal_mix_tool**: Determines the best combination of projects to maximize return for a specific risk level and budget
- **evaluate_strategic_alignment_tool**: Checks how well the chosen portfolio meets high-level corporate goals
- **simulate_risk_scenarios_tool**: Tests the robustness of a selected project mix against various market volatility levels
- **analyze_project_inventory_tool**: Evaluates the available pool of projects to ensure they meet minimum viability standards


## 💬 Prompt Examples

Here are some examples of how you can interact with the **E&P Portfolio Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this list of projects and tell me which ones are viable: [{'id': 'P1', 'expected_return': 0.15, 'required_capital': 100, 'risk': 0.05}, {'id': 'P2', 'expected_return': -0.05, 'required_capital': 50, 'risk': 0.1}]"

**🤖 AI Agent:**
> The viable projects are P1. Project P2 is excluded because it has a negative expected return.

---

**👤 You:**
> "Find the best project mix for a budget of 500 and a risk tolerance of 0.1 using these projects: [{'id': 'A', 'expected_return': 0.2, 'required_capital': 200, 'risk': 0.05}, {'id': 'B', 'expected_return': 0.25, 'required_capital': 350, 'risk': 0.15}]"

**🤖 AI Agent:**
> The optimal mix includes project A. Total expected return is 0.2 with a total capital used of 200.

---

**👤 You:**
> "What happens to my portfolio if market volatility doubles?"

**🤖 AI Agent:**
> With a volatility multiplier of 2.0, your worst-case return is projected to be -12% and the probability of loss increases to 15%.


## ❓ FAQ

**Q: How does the tool handle budget constraints?**
The `calculate_optimal_mix_tool` ensures that the sum of capital required for all selected projects does not exceed the specified budget limit.

**Q: Can I test how my portfolio performs in a market crash?**
Yes, you can use `simulate_risk_scenarios_tool` to apply a volatility multiplier to your selected projects and see the potential impact on returns.

**Q: How do I ensure my portfolio meets ESG targets?**
You can use `evaluate_strategic_alignment_tool` to check your project mix against specific criteria like ESG scores or geographic requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ep-portfolio-optimizer](https://vinkius.com/ai-agent-connect/ep-portfolio-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **E&P Portfolio Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ep-portfolio-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **E&P Portfolio Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ep-portfolio-optimizer": {
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
