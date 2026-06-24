# Portfolio Concentration Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/portfolio-concentration-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Measure investment risk using the Herfindahl-Hirschman Index (HHI) across asset, sector, and geography dimensions.

## Description
This MCP server provides a specialized engine for analyzing portfolio diversification. By using the `calculate_concentration_metrics` tool, you can compute the Herfindahl-Hirschman Index (HHI) to identify concentration risks within your holdings at the asset, sector, and geography levels. The server also includes `get_diversification_recommendation` to provide actionable advice on rebalancing highly concentrated dimensions and `validate_portfolio_data` to ensure your input data is mathematically sound for HHI calculations.


## Available Tools (3)
- **calculate_concentration_metrics**: Calculates HHI and concentration metrics
- **get_diversification_recommendation**: Gets diversification recommendations
- **validate_portfolio_data**: Validates the input portfolio data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Portfolio Concentration Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the concentration metrics for a portfolio with 50% Apple (Tech, USA), 30% Microsoft (Tech, USA), and 20% Tesla (Auto, USA)."

**🤖 AI Agent:**
> The analysis shows a high concentration in the Technology sector (HHI: 0.34) and the USA geography (HHI: 1.0). The Sector rating is 'Concentrated'.

---

**👤 You:**
> "What should I do to diversify my portfolio if my sector concentration is too high?"

**🤖 AI Agent:**
> To reduce risk, you should redistribute weight from your most concentrated sectors into underrepresented industries like Healthcare or Energy.

---

**👤 You:**
> "Check if my portfolio data is valid: [{'weight': 0.5, 'sector': 'Tech', 'geography': 'USA'}, {'weight': -0.1, 'sector': 'Energy', 'geography': 'UK'}]"

**🤖 AI Agent:**
> The validation failed because the asset with weight -0.1 has an invalid negative value.


## ❓ FAQ

**Q: What is the Herfindahl-Hirschman Index (HHI)?**
The HHI is a standard economic metric used to measure market or portfolio concentration. It is calculated by squaring the weight of each component and summing the results.

**Q: How can I identify which part of my portfolio is too concentrated?**
You can use the `calculate_concentration_metrics` tool to see HHI scores and ratings for assets, sectors, and geographies. If a dimension shows a 'Concentrated' rating, it indicates high risk.

**Q: Does the tool provide advice on how to fix concentration?**
Yes, by using the `get_diversification_recommendation` tool, you can receive specific instructions on which sectors or regions to reduce exposure to in order to improve diversification.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/portfolio-concentration-calculator](https://vinkius.com/mcp/portfolio-concentration-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Portfolio Concentration Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `portfolio-concentration-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Portfolio Concentration Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "portfolio-concentration-calculator": {
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
