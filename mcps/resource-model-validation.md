# Resource Model Validation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/resource-model-validation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analysis](../categories/data-analysis.md)

Validate mineral resource block models using statistical analysis and spatial swath plots.

## Description
This MCP server provides a specialized toolset for evaluating the accuracy and reliability of mineral resource block models. It allows for direct comparison between estimated model grades and measured sample data. Users can perform global statistical comparisons using `get_statistical_summary`, evaluate spatial accuracy through `generate_swath_analysis`, compute advanced error metrics with `calculate_validation_metrics`, and pinpoint geographic discrepancies using `detect_local_bias`.


## Available Tools (4)
- **calculate_validation_metrics**: Computes advanced error metrics to quantify model quality
- **detect_local_bias**: Identifies specific geographic areas where the model is significantly overestimating or underestimating
- **generate_swath_analysis**: Evaluates the spatial accuracy of the model by comparing averages along a chosen axis
- **get_statistical_summary**: Provides a high-level comparison of the globalThis averages between the model and the samples


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Resource Model Validation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare the global averages of these sample grades [12.5, 13.2, 11.8] and model grades [12.8, 13.0, 12.1]."

**🤖 AI Agent:**
> The model mean is 12.63 and the sample mean is 12.5. The mean difference is -0.13, indicating a slight overestimation by the model.

---

**👤 You:**
> "Calculate the validation metrics for sample grades [10.0, 15.0] and model grades [11.0, 14.0]."

**🤖 AI Agent:**
> The RMSE is 1.0, the mean error is 0.0, and the relative error is 0.0.

---

**👤 You:**
> "Run a swath analysis along the Z axis with 5 slices using the provided points."

**🤖 AI Agent:**
> The swath analysis along the Z axis is complete. The maximum deviation across the 5 slices is 0.45 grade units.


## ❓ FAQ

**Q: How can I check for systematic errors in my model?**
You can use `calculate_validation_metrics` to compute RMSE and mean error, or `detect_local_bias` to find specific geographic zones where the model deviates from sample data.

**Q: What is the purpose of swath analysis?**
The `generate_swath_analysis` tool evaluates spatial accuracy by comparing average grades along a chosen axis (X, Y, or Z) within defined slices.

**Q: Does this tool handle sampling bias?**
Yes, the `get_statistical_summary` tool includes an option to apply declustering weights to correct for sampling bias.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/resource-model-validation](https://vinkius.com/ai-agent-connect/resource-model-validation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Resource Model Validation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `resource-model-validation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Resource Model Validation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "resource-model-validation": {
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
