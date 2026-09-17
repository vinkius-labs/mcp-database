# Wine Bottle Variation Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-bottle-variation-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predicts bottle-to-bottle variation and quality windows using stochastic oxygen ingress modeling.

## Description
This MCP server provides a predictive analysis engine to model how oxygen ingress affects wine quality over time. By accounting for closure lot variation, fill height, and storage orientation, it helps predict the expected variation in oxygen exposure and identifies the optimal drinking window for a batch of bottles. Use `predict_variation_at_age` to calculate quality deviation, `calculate_quality_outliers` to find the percentage of bottles outside quality limits, `get_optimal_drinking_window` to identify peak quality years, and `simulate_storage_impact` to compare horizontal versus vertical storage effects.


## Available Tools (4)
- **calculate_quality_outliers**: Determines the percentage of bottles in a batch that are expected to fall outside the acceptable quality limits at a given time
- **get_optimal_drinking_window**: Identifies the time range during which the most bottles are expected to be in their peak quality state
- **predict_variation_at_age**: Calculates the expected range of oxygen exposure and quality deviation for a group of bottles at a specific point in time
- **simulate_storage_impact**: Compares how different storage orientations affect the rate of variation for a specific closure type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Bottle Variation Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected quality deviation for natural cork bottles stored horizontally after 10 years?"

**🤖 AI Agent:**
> At 10 years, the expected quality deviation for natural cork bottles stored horizontally is 0.12 with a mean oxygen exposure of 4.5 mg/L.

---

**👤 You:**
> "How many bottles will likely be bad after 20 years if I use screwcaps?"

**🤖 AI Agent:**
> With screwcap closures, the predicted percentage of bottles falling outside the quality threshold after 20 years is 0.05%.

---

**👤 You:**
> "Compare horizontal and vertical storage for natural cork at 5 years."

**🤖 AI Agent:**
> For natural cork at 5 years, horizontal storage results in a variation of 0.45, while vertical storage results in 0.32, yielding an impact ratio of 1.41.


## ❓ FAQ

**Q: How does storage position affect the prediction?**
Storage position (horizontal vs vertical) changes the contact surface area between the liquid and the closure, which directly influences the oxygen ingress rate modeled by the tools.

**Q: Can I use this to find the best time to drink a specific vintage?**
Yes, by using `get_optimal_drinking_window`, you can identify the specific age range where the majority of bottles are predicted to be in their peak quality state.

**Q: What is the purpose of the `calculate_quality_outliers` tool?**
The `calculate_quality_outliers` tool determines the percentage of bottles in a batch expected to fall outside acceptable oxygen exposure limits at a given age.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-bottle-variation-predictor](https://vinkius.com/en/ai-agent-connect/wine-bottle-variation-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Bottle Variation Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-bottle-variation-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Bottle Variation Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-bottle-variation-predictor": {
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
