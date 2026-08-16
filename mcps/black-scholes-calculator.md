# Black-Scholes Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/black-scholes-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic engine for European option pricing and Greeks sensitivity analysis.

## Description
This MCP server provides a deterministic mathematical engine for European-style option pricing. It allows AI agents to calculate the theoretical fair value of options and their sensitivities, known as Greeks, using the Black-Scholes model. Users can utilize `calculate_option_price` to find the exact price of a call or put, `calculate_option_greeks` to determine Delta, Gamma, Vega, Theta, and Rho, or `validate_market_data` to ensure input parameters are within realistic bounds.


## Available Tools (3)
- **calculate_option_greeks**: Calculates the sensitivities (Greeks) of an option
- **calculate_option_price**: Calculates the theoretical fair value of a European option
- **validate_market_data**: Ensures that the provided market parameters are within realistic, non-negative bounds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Black-Scholes Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the price of a call option with an underlying price of 100, strike of 100, 1 year to expiry, 5% risk-free rate, and 20% volatility?"

**🤖 AI Agent:**
> The theoretical price for this call option is 10.45.

---

**👤 You:**
> "Calculate the Greeks for a put option: underlying 100, strike 105, 0.5 years to expiry, 3% risk-free rate, and 25% volatility."

**🤖 AI Agent:**
> The Greeks for this put option are: Delta -0.42, Gamma 0.03, Vega 0.28, Theta -0.05, and Rho -0.12.

---

**👤 You:**
> "Is a volatility of -0.05 valid for pricing?"

**🤖 AI Agent:**
> No, volatility must be a positive value.


## ❓ FAQ

**Q: What models are used for pricing?**
The server uses the standard Black-Scholes model for European-style options.

**Q: Can I calculate Greeks?**
Yes, by using the `calculate_option_greeks` tool, you can obtain Delta, Gamma, Vega, Theta, and Rho.

**Q: How do I ensure my inputs are valid?**
You can use the `validate_market_data` tool to check if your parameters like volatility and price are within realistic bounds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/black-scholes-calculator](https://vinkius.com/ai-agent-connect/black-scholes-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Black-Scholes Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `black-scholes-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Black-Scholes Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "black-scholes-calculator": {
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
