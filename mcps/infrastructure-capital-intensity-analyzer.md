# Infrastructure Capital Intensity Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/infrastructure-capital-intensity-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Analyze capital intensity, spending splits, and asset efficiency for infrastructure businesses.

## Description
This MCP server provides specialized financial modeling tools for infrastructure-heavy businesses. It allows AI agents to calculate the relationship between capital investment and revenue, determine the split between Capex and Opex, and evaluate how effectively an asset base is being utilized. Use `analyze_capital_intensity` to find the capital intensity level, `calculate_spending_split` to compare growth vs maintenance spending, `evaluate_asset_efficiency` to assess asset turnover, and `project_reinvestment_needs` to estimate future capital requirements for maintaining assets.


## Available Tools (4)
- **analyze_capital_intensity**: Provides a high-level overview of the relationship between capital investment and revenue generation
- **calculate_spending_split**: Compares the amount spent on maintaining operations versus growing the asset base
- **evaluate_asset_efficiency**: Determines how effectively the current asset base is producing revenue while accounting for the cost of asset aging
- **project_reinvestment_needs**: Estimates the future capital required to maintain the current asset base as existing assets depreciate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Infrastructure Capital Intensity Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the capital intensity for a company with $50M annual Capex and $200M annual revenue?"

**🤖 AI Agent:**
> The capex-to-revenue ratio is 25%, which indicates a High capital intensity level.

---

**👤 You:**
> "Compare the spending split for $10M Capex and $40M Opex."

**🤖 AI Agent:**
> The total spend is $50M, with Capex accounting for 20% and Opex accounting for 80% of the total expenditure.

---

**👤 You:**
> "How efficient is an asset base of $100M generating $20M in revenue with a 10-year depreciation schedule?"

**🤖 AI Agent:**
> The asset turnover is 0.2, and the capital efficiency score is calculated based on the depreciation impact of the 10-year schedule.


## ❓ FAQ

**Q: How do I calculate the capital intensity level?**
You can use the `analyze_capital_intensity` tool by providing the annual Capex and annual revenue.

**Q: Can I estimate future capital needs?**
Yes, the `project_reinvestment_needs` tool estimates the annual replacement requirement to maintain your asset base.

**Q: What is the difference between Capex and Opex in this tool?**
Capex refers to capital expenditures for assets, while Opex refers to operating expenditures. The `calculate_spending_split` tool helps you see the percentage distribution between the two.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/infrastructure-capital-intensity-analyzer](https://vinkius.com/en/ai-agent-connect/infrastructure-capital-intensity-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Infrastructure Capital Intensity Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `infrastructure-capital-intensity-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Infrastructure Capital Intensity Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "infrastructure-capital-intensity-analyzer": {
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
