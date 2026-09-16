# Venture Market Size Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-market-size-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Validates market size claims using top-down and bottom-up methodologies.

## Description
This MCP server provides specialized tools to verify market sizing accuracy. It reconciles top-down and bottom-up estimates to provide a validated TAM range and a confidence score. Use `validate_market_claims` to check the alignment of your market figures, `calculate_market_penetration` to assess if your target capture is realistic, `analyze_growth_impact` for future projections, and `get_market_segmentation_sanity` to ensure your TAM, SAM, and SOM hierarchy is logically sound.


## Available Tools (4)
- **get_market_segmentation_sanity**: Checks if the hierarchy of TAM, SAM, and SOM is logically consistent
- **validate_market_claims**: Reconciles top-down and bottom-up estimates to provide a validated range and confidence assessment
- **analyze_growth_impact**: Forecasts how the market size evolves over a given period based on growth rates
- **calculate_market_penetration**: Evaluates if the SOM is a realistic subset of the SAM based on competitive landscape


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Market Size Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate these market claims: TAM is $10B, SAM is $2B, SOM is $500M, growth is 5%, and market dynamics score is 0.8. The bottom-up TAM is $9B."

**🤖 AI Agent:**
> The validated TAM range is $9.5B, with an achievable market share of 25% and a confidence score of 85%.

---

**👤 You:**
> "Is a SOM of $100M realistic for a SAM of $500M with a competitive intensity of 0.7?"

**🤖 AI Agent:**
> The penetration rate is 20%, and the feasibility rating is Medium due to the high competitive intensity.

---

**👤 You:**
> "Project a TAM of $1B with a 10% annual growth rate over 5 years."

**🤖 AI Agent:**
> The projected TAM after 5 years is $1.61B.


## ❓ FAQ

**Q: How does the tool validate market claims?**
The `validate_market_claims` tool compares your top-down estimates against bottom-up data to calculate a confidence score and a reconciled TAM range.

**Q: Can I check if my market hierarchy is logical?**
Yes, use `get_market_segmentation_sanity` to verify that your TAM, SAM, and SOM follow the required hierarchy.

**Q: How do I forecast future market size?**
You can use `analyze_growth_impact` to project the TAM over a specific number of years based on an annual growth rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-market-size-validator](https://vinkius.com/en/ai-agent-connect/venture-market-size-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Market Size Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-market-size-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Market Size Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-market-size-validator": {
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
