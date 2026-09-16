# Reservoir Prediction Uncertainty MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/reservoir-prediction-uncertainty)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Quantifies uncertainty in reservoir predictions using parameter ranges and correlations.

## Description
This MCP server provides tools to quantify uncertainty in reservoir engineering predictions. By propagating parameter ranges and accounting for correlations, it calculates confidence intervals, identifies key uncertainty drivers, and generates statistical summaries of probability distributions. Use `calculate_prediction_intervals` to find likely outcome ranges, `identify_uncertainty_drivers` to find high-impact parameters, and `generate_distribution_summary` for statistical insights.


## Available Tools (4)
- **calculate_prediction_intervals**: Calculates prediction intervals using parameter ranges and correlations
- **generate_distribution_summary**: Generates a statistical summary of a probability distribution
- **identify_uncertainty_drivers**: Identifies key uncertainty drivers by ranking sensitivity
- **validate_parameter_consistency**: Validates if parameter ranges and correlations are logically compatible


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reservoir Prediction Uncertainty** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the range of likely outcomes for my reservoir prediction given these parameters?"

**🤖 AI Agent:**
> The predicted fluid recovery range is between 1.2 million and 1.8 million barrels at a 95% confidence level.

---

**👤 You:**
> "Which parameters are the main drivers of uncertainty in this model?"

**🤖 AI Agent:**
> The primary uncertainty drivers are porosity and permeability.

---

**👤 You:**
> "Give me a summary of this probability distribution."

**🤖 AI Agent:**
> The distribution has a mean of 1.5 million, a median of 1.48 million, and a standard deviation of 0.15 million.


## ❓ FAQ

**Q: How do I calculate the range of likely outcomes?**
You can use the `calculate_prediction_intervals` tool by providing your parameter ranges and any existing correlations.

**Q: How can I find which parameters impact my model most?**
Use the `identify_uncertainty_drivers` tool to rank parameters based on their sensitivity scores.

**Q: Can I check if my input data is logically consistent?**
Yes, the `validate_parameter_consistency` tool checks if your parameter ranges and correlations are physically and logically compatible.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/reservoir-prediction-uncertainty](https://vinkius.com/en/ai-agent-connect/reservoir-prediction-uncertainty)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reservoir Prediction Uncertainty** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reservoir-prediction-uncertainty` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reservoir Prediction Uncertainty** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reservoir-prediction-uncertainty": {
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
