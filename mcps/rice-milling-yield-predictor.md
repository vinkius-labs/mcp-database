# Rice Milling Yield Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/rice-milling-yield-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Predicts rice milling quality and economic output from kernel traits.

## Description
This MCP server provides specialized tools to predict rice milling quality and economic value. By analyzing kernel geometry, chalkiness, and moisture levels, users can determine Head Rice Yield (HRY) and assess breakage risks. Use `predict_yield_metrics` to calculate physical outcomes, `calculate_economic_value` for monetary projections, `assess_fissuring_risk` to evaluate structural stability, and `get_variety_reference` to retrieve genetic resilience coefficients.


## Available Tools (4)
- **assess_fissuring_risk**: Evaluates the likelihood of grain breakage due to moisture-related structural failure
- **calculate_economic_value**: Determines the monetary value of the milled rice based on its quality grades
- **get_variety_reference**: Retrieves the standard milling potential coefficient for a specific rice variety
- **predict_yield_metrics**: Calculates the primary physical yield outcomes for a given sample of rice


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rice Milling Yield Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the predicted yield for a rice sample with length 7mm, width 2mm, thickness 2mm, 15% chalkiness, 18% moisture, and a variety potential of 0.85?"

**🤖 AI Agent:**
> The predicted head rice yield is 72%, with a broken kernel percentage of 18% and a total milling yield of 90%.

---

**👤 You:**
> "Calculate the economic value for a yield with 75% head rice, 15% broken rice, and a Premium grade."

**🤖 AI Agent:**
> The total economic value is $450.00 with a Premium grade classification.

---

**👤 You:**
> "What is the fissuring risk for rice with 22% moisture and 25% chalkiness?"

**🤖 AI Agent:**
> The risk level is High with a breakage probability of 0.78.


## ❓ FAQ

**Q: What data is required for yield prediction?**
You need to provide kernel length, width, thickness, chalkiness percentage, moisture content, and the variety's milling potential.

**Q: How is the economic value determined?**
The value is calculated using `calculate_economic_value` based on the head rice yield, broken kernel percentage, and the selected market price grade.

**Q: Can I check the risk of grain breakage?**
Yes, use the `assess_fissuring_risk` tool to evaluate the likelihood of breakage based on moisture and chalkiness.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/rice-milling-yield-predictor](https://vinkius.com/ai-agent-connect/rice-milling-yield-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rice Milling Yield Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rice-milling-yield-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rice Milling Yield Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rice-milling-yield-predictor": {
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
