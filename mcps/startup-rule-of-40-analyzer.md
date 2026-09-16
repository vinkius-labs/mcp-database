# Startup Rule of 40 Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/startup-rule-of-40-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Evaluate SaaS financial health by balancing growth and profitability.

## Description
This MCP server provides essential financial health assessment tools for software companies. It allows AI agents to calculate the Rule of 40 score, which balances year-over-year revenue growth against EBITDA margin. Using `calculate_rule_of_40`, agents can determine a company's balance type and adjusted score based on maturity and market conditions. Additionally, `get_benchmark_comparison` provides performance tiering, while `evaluate_growth_profit_tradeoff` and `get_market_sensitivity_analysis` offer deep insights into strategic positioning and economic resilience.


## Available Tools (4)
- **calculate_rule_of_40**: Calculates the Rule of 40 score, balance type, and adjusted score
- **evaluate_growth_profit_tradeoff**: Evaluates the tradeoff between growth and profit based on company stage
- **get_benchmark_comparison**: Compares a Rule of 40 score against industry standards
- **get_market_sensitivity_analysis**: Analyzes how sensitive the score is to market conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Startup Rule of 40 Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the Rule of 40 score for a company with 30% growth and 15% EBITDA margin?"

**🤖 AI Agent:**
> The Rule of 40 score is 45, which indicates a healthy and efficient business model.

---

**👤 You:**
> "Compare a score of 35 against industry benchmarks."

**🤖 AI Agent:**
> A score of 35 is classified as 'Average' and falls just below the typical healthy threshold of 40.

---

**👤 You:**
> "Is a company with 50% growth and -5% EBITDA margin prioritizing growth too aggressively for an early-stage company?"

**🤖 AI Agent:**
> The tradeoff profile is 'Aggressive Growth', which is common for early-stage companies prioritizing market capture over immediate profit.


## ❓ FAQ

**Q: What is the Rule of 40?**
The Rule of 40 is a metric used to evaluate the health of SaaS companies by summing their revenue growth rate and EBITDA margin.

**Q: How can I compare my score to industry standards?**
You can use the `get_benchmark_comparison` tool to receive a performance tier classification and see if your score meets healthy thresholds.

**Q: Does the tool account for different company stages?**
Yes, the `calculate_rule_of_40` tool includes a `companyStage` parameter to adjust the score based on whether a company is early-stage, growth-stage, or mature.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/startup-rule-of-40-analyzer](https://vinkius.com/en/ai-agent-connect/startup-rule-of-40-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Startup Rule of 40 Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `startup-rule-of-40-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Startup Rule of 40 Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "startup-rule-of-40-analyzer": {
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
