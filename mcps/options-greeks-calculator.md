# Options Greeks Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/options-greeks-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Black-Scholes theoretical option prices and Greeks (Delta, Gamma, Theta, Vega, Rho) to assess market risk.

## Description
This MCP server provides a high-precision financial engine for calculating European-style option prices and their sensitivities using the Black-Scholes model. By connecting your AI agent to this tool, you can instantly quantify market risks such as price movements (`calculate_directional_risk`), time decay via `calculate_environmental_sensitivities`, and theoretical fair value through `calculate_option_valuation`. It is designed for traders and analysts who need to assess how changes in underlying price, volatility, interest rates, and time until expiration impact their option positions.


## Available Tools (3)
- **calculate_directional_risk**: Quantifies how much the option price reacts to movements in the underlying asset's price
- **calculate_environmental_sensitivities**: Quantifies how external factors like time, volatility, and interest rates impact the option's value
- **calculate_option_valuation**: Calculates Black-Scholes theoretical prices for Call and Put options


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Options Greeks Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the theoretical price for a Call option with an underlying price of 100, strike of 105, 0.5 years to expiry, 5% risk-free rate, and 20% volatility?"

**🤖 AI Agent:**
> The theoretical Call price is approximately 4.37.

---

**👤 You:**
> "Calculate the directional risk for an option with underlying at 150, strike at 145, 0.2 years left, 3% rate, and 30% volatility."

**🤖 AI Agent:**
> The Delta is 0.68 and Gamma is 0.025, indicating a moderately aggressive directional exposure.

---

**👤 You:**
> "How much value will my option lose per day due to time decay?"

**🤖 AI Agent:**
> Based on the provided parameters, your daily Theta is -0.05, meaning the option loses approximately 0.05 in value every day.


## ❓ FAQ

**Q: What is the purpose of the `calculate_option_valuation` tool?**
It determines the theoretical fair market price for both Call and Put options based on inputs like underlying price, strike, time to expiry, risk-free rate, and volatility.

**Q: How can I assess the impact of volatility changes?**
Use the `calculate_environmental_sensitivities` tool to find the Vega, which measures price sensitivity to a 1% change in implied volatility.

**Q: Does this tool handle directional risk?**
Yes, the `calculate_directional_risk` tool quantifies Delta and Gamma to show how much your option price reacts to movements in the underlying asset's price.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/options-greeks-calculator](https://vinkius.com/mcp/options-greeks-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Options Greeks Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `options-greeks-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Options Greeks Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "options-greeks-calculator": {
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
