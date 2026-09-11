# Infrastructure Fund Appeal Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/infrastructure-fund-appeal-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Quantifies the attractiveness and suitability of infrastructure funds for various investor classes.

## Description
This MCP server provides a specialized financial analysis engine to evaluate infrastructure investments. It calculates a comprehensive fund appeal score by analyzing yield, inflation linkage, contract duration, and risk profiles. Using tools like `get_fund_appeal_score` and `get_investor_suitability`, it identifies the best-fit investor types--such as Pension Funds or Sovereign Wealth Funds--and assesses downside protection against economic volatility. It is designed to help institutional investors quantify the real value and risk-adjusted returns of infrastructure assets.


## Available Tools (4)
- **evaluate_downside_protection**: Assesses how well the fund protects against adverse economic conditions
- **get_fund_appeal_score**: Calculates the primary attractiveness score for a specific infrastructure fund
- **get_investor_suitability**: Determines the most appropriate class of investor for the given fund parameters
- **get_yield_profile_details**: Provides a detailed qualitative description of the fund's yield characteristics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Infrastructure Fund Appeal Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the appeal score for a fund with 5% yield, 0.8 inflation linkage, 15 year duration, low risk, and an ESG score of 85."

**🤖 AI Agent:**
> The fund has an appeal score of 88, a stable yield profile, and is a primary match for Pension Funds.

---

**👤 You:**
> "What is the suitability for a fund with a 20-year duration, high risk, and an ESG score of 60?"

**🤖 AI Agent:**
> This fund is best suited for Private Equity due to its high risk profile and specific duration characteristics.

---

**👤 You:**
> "Check the downside protection for a fund with 0.2 inflation linkage and high risk."

**🤖 AI Agent:**
> The protection strength is low, indicating a high vulnerability to inflation and market volatility.


## ❓ FAQ

**Q: How is the fund appeal score calculated?**
The score is a composite metric derived from the `get_fund_appeal_score` tool, which weighs annual yield, inflation linkage, contract duration, risk profile, and ESG ratings.

**Q: Can I determine which investor type is best for a fund?**
Yes, the `get_investor_suitability` tool analyzes contract duration, risk, and ESG scores to recommend the most appropriate investor class, such as Pension Funds or Insurance Companies.

**Q: Does the tool account for inflation protection?**
Yes, the `evaluate_downside_protection` tool specifically assesses how inflation linkage and risk profiles protect the fund against adverse economic conditions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/infrastructure-fund-appeal-analyzer](https://vinkius.com/en/ai-agent-connect/infrastructure-fund-appeal-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Infrastructure Fund Appeal Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `infrastructure-fund-appeal-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Infrastructure Fund Appeal Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "infrastructure-fund-appeal-analyzer": {
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
