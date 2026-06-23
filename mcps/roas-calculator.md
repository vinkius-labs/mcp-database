# ROAS Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/roas-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Accurately determine your Return on Ad Spend (ROAS) across all channels, benchmark against industry standards, and calculate the break-even point to guide profitable ad spending.

## Description
# Assess Advertising Profitability with Precision

The challenge for any growing business is knowing if money spent on advertising actually generates profit. Many companies struggle to connect their media spend (ad cost) directly to the long-term revenue generated, leading to inefficient spending and guesswork in scaling campaigns.

Our MCP provides a structured mechanism to bridge this financial intelligence gap by running three sequential, interconnected calculations:

1. **Calculate Total ROAS:** We start by using `calculate_roas`. You input your total media spend and the attributed revenue. This tool calculates the overall Return on Ad Spend (ROAS) and can provide a detailed breakdown by specific channels or individual campaigns.
2. **Benchmark Performance:** Next, we use `get_target_benchmark` to establish an industry-standard floor. By specifying your business type (e.g., E-commerce, SaaS), the tool returns the minimum required ROAS benchmark, ensuring you measure performance against best practices.
3. **Determine Break-Even Point:** Finally, using `calculate_break_even_roas`, you input your contribution margin percentage. This calculates the absolute minimum ROAS needed just to cover all marginal costs associated with ad spend, giving you a safety net threshold.

The result is not just a number; it's an actionable blueprint for financial health. By systematically linking what was spent (`calculate_roas`), what *should* have been achieved (`get_target_benchmark`), and the minimum sustainable performance level (`calculate_break_even_roas`), you can immediately determine if your marketing spend supports profitable growth.


## Available Tools (3)
- **calculate_break_even_roas**: Calculate the minimum ROAS needed to break even given a contribution margin
- **calculate_roas**: Provide mediaSpend and sourceRevenue for the calculation.

Calculate Return on Ad Spend (ROAS) with optional channel/campaign breakdown
- **get_target_benchmark**: Get the target ROAS benchmark for a specific business type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ROAS Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We spent $15,000 last month and generated $60,000 in revenue. Can you calculate the total ROAS and break down the performance by 'Google Ads' vs 'Facebook/Instagram'?"

**🤖 AI Agent:**
> Calling `calculate_roas` with mediaSpend=15000, sourceRevenue=60000, and groupByField='Channel'. The total ROAS is 4.0x. Google Ads contributed a ROAS of X, while Facebook/Instagram contributed Y.

---

**👤 You:**
> "We are an E-commerce company reporting in USD. What is the minimum target ROAS we should aim for?"

**🤖 AI Agent:**
> Calling `get_target_benchmark` with businessType='E-commerce' and targetCurrencyCode='USD'. The system returns a benchmark of 4x, which serves as your minimum performance goal.

---

**👤 You:**
> "Our current contribution margin is 0.55 (55%). What ROAS do we need to break even in EUR?"

**🤖 AI Agent:**
> Calling `calculate_break_even_roas` with contributionMarginPercentage=0.55 and targetCurrencyCode='EUR'. The required break-even ROAS is 1.82x, meaning your ad spend must generate at least this much revenue to cover all marginal costs.


## ❓ FAQ

**Q: What is the difference between overall ROAS and channel-specific ROAS?**
You can use `calculate_roas` to get both. By providing a 'groupByField' (like Channel), the tool calculates the total ROAS across all inputs, but also provides granular performance metrics for each distinct channel or campaign group.

**Q: How do I know if my benchmark is appropriate?**
The `get_target_benchmark` tool requires your business type (E-commerce, SaaS, etc.) and currency code. It returns the industry standard for that segment, helping you compare your calculated ROAS against a recognized best practice.

**Q: What if my business has high fixed costs?**
While the tool primarily uses contribution margin, you can use `calculate_break_even_roas` to model profitability. By accurately reporting your contribution margin percentage, it determines the minimum ROAS needed to cover all marginal costs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/roas-calculator](https://vinkius.com/mcp/roas-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ROAS Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `roas-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ROAS Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "roas-calculator": {
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
