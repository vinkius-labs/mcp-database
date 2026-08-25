# Accelerator Portfolio Concentration Risk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-portfolio-concentration-risk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Quantify capital exposure and diversification health for accelerator funds.

## Description
This MCP server provides specialized risk analysis for accelerator funds. It allows AI agents to quantify capital exposure across sectors, investment stages, and individual company concentrations. Using the Herfindahl-Hirschman Index (HHI), the server calculates how concentrated capital is within specific companies and industries. It also provides a holistic diversification score that accounts for sector spread, stage distribution, and correlation factors to assess the overall health of a portfolio.


## Available Tools (3)
- **analyze_sector_exposure**: Analyze portfolio exposure across different sectors
- **evaluate_portfolio_diversification**: Evaluate overall portfolio diversification health
- **calculate_hhi_index**: Calculate the Herfindahl-Hirschman Index (HHI) for a list of investments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Portfolio Concentration Risk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the HHI for these investments: [100000, 200000, 700000]"

**🤖 AI Agent:**
> The calculated HHI index is 0.54, which indicates a moderate concentration level.

---

**👤 You:**
> "Analyze my sector exposure with this map: {"Fintech": 500000, "SaaS": 300000, "AI": 200000}"

**🤖 AI Agent:**
> The sector concentration is 0.38, with Fintech being the dominant sector. The risk rating is Diversified.

---

**👤 You:**
> "What is my diversification score for investments [500, 500], sectors {"Tech": 1000}, stages {"Seed": 1000}, and a correlation of 0.2?"

**🤖 AI Agent:**
> The diversification score is 85, representing a Balanced risk profile. The exposure summary indicates a well-distributed portfolio.


## ❓ FAQ

**Q: How is the HHI calculated?**
The `calculate_hhi_index` tool calculates the index by squaring the percentage share of each company's investment relative to the total fund value and summing those squares.

**Q: Can I analyze sector-specific risks?**
Yes, you can use `analyze_sector_exposure` to identify if your portfolio is over-exposed to a single industry and find your dominant sector.

**Q: What factors influence the diversification score?**
The `evaluate_portfolio_diversification` tool calculates a score based on investment distribution, sector spread, stage spread, and a correlation factor representing the relationship between companies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-portfolio-concentration-risk](https://vinkius.com/ai-agent-connect/accelerator-portfolio-concentration-risk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Portfolio Concentration Risk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-portfolio-concentration-risk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Portfolio Concentration Risk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-portfolio-concentration-risk": {
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
