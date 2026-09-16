# Venture Angel Investment Sizing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-angel-investment-sizing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Strategic decision-support for angel investors to optimize portfolio allocation and follow-on reserves.

## Description
This MCP server provides critical decision-support tools for angel investors to manage capital allocation through the lens of power law dynamics. It allows investors to model their entire lifecycle by using `calculate_portfolio_structure` to split capital between initial checks and reserves. Users can model specific investment tiers with `generate_check_size_distribution`, ensure they have enough dry powder to defend winners using `evaluate_followon_capacity`, and assess concentration risk via `analyze_capital_efficiency`. It is designed to help investors balance diversification targets against the need for high-impact follow-on participation.


## Available Tools (4)
- **analyze_capital_efficiency**: Measures the relationship between initial deployment and total potential exposure to assess concentration
- **evaluate_followon_capacity**: Analyzes whether the current reserve allocation is sufficient to maintain ownership in winners
- **generate_check_size_distribution**: Provides a detailed breakdown of how many checks can be written at various tiers within a user-defined range
- **calculate_portfolio_structure**: Determines the high-level breakdown of how capital is split between initial checks and follow-on reserves


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Angel Investment Sizing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have $1,000,000 for an angel fund. I want to invest in 20 companies and keep 40% for follow-on reserves. What is my initial deployment and average check size?"

**🤖 AI Agent:**
> With a $1,000,000 portfolio and a 40% reserve, your initial deployment is $600,000 and your reserve amount is $400,000. The average initial check size for 20 companies is $30,000.

---

**👤 You:**
> "If I have $400,000 in reserves for 20 companies and expect 2 winners that need follow-on, is my reserve enough?"

**🤖 AI Agent:**
> Yes, with $400,000 in reserves and 2 expected winners, you have a maximum of $200,000 available for each winning company.

---

**👤 You:**
> "Calculate the efficiency and concentration risk for a $500,000 portfolio with $450,000 initial deployment and 25 companies."

**🤖 AI Agent:**
> The efficiency ratio is 0.9 and the concentration risk score is High, as most of your capital is deployed in the initial round.


## ❓ FAQ

**Q: How does this tool help with power law returns?**
The tool uses `evaluate_followon_capacity` to ensure that your reserve allocation is sufficient to support the few 'winners' that typically drive power law returns in an angel portfolio.

**Q: Can I model different check size strategies?**
Yes, you can use `generate_check_size_distribution` to see how your initial deployment can be spread across different investment tiers within your minimum and maximum bounds.

**Q: How is concentration risk measured?**
Concentration risk is assessed using `analyze_capital_efficiency`, which compares your initial deployment to your total portfolio size to determine if your strategy is too concentrated or sufficiently diversified.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-angel-investment-sizing](https://vinkius.com/en/ai-agent-connect/venture-angel-investment-sizing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Angel Investment Sizing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-angel-investment-sizing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Angel Investment Sizing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-angel-investment-sizing": {
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
