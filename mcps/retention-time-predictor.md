# Retention Time Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/retention-time-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Predict chromatography retention times, capacity factors, and selectivity using QSRR.

## Description
This MCP server provides advanced chromatographic modeling using Quantitative Structure-Retention Relationships (QSRR). It allows AI agents to calculate expected retention times, capacity factors, and selectivity for specific compounds based on molecular structure, column properties, and mobile phase composition. Use `predict_retention_time` to estimate elution timing, `calculate_selectivity` to evaluate separation efficiency between analytes, `analyze_gradient_efficiency` to model gradient elution profiles, and `compare_column_performance` to optimize stationary phase selection.


## Available Tools (4)
- **analyze_gradient_efficiency**: Evaluate how a change in mobile phase composition (gradient) impacts the elution profile
- **calculate_selectivity**: Determine how well two different compounds can be separated by a specific chromatographic setup
- **compare_column_performance**: Predict how switching between different column types will change the retention behavior for a set of compounds
- **predict_retention_time**: Calculate the expected retention time for a specific compound under defined chromatographic conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Retention Time Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the retention time for Caffeine (CC1=NC=C(N1)C(=O)N) using a C18 column (150mm, 5um) and a mobile phase with 40% acetonitrile at 25 degrees Celsius."

**🤖 AI Agent:**
> The predicted retention time for Caffeine is 8.42 minutes, with a capacity factor of 2.15.

---

**👤 You:**
> "How well can I separate Benzene (C1=CC=CC=C1) and Toluene (CC1=CC=CC=C1) using a Silica column?"

**🤖 AI Agent:**
> The selectivity alpha for Benzene and Toluene on this Silica column is 1.45, indicating a good separation.

---

**👤 You:**
> "Analyze the efficiency of a gradient elution for Aspirin (CC(=O)OC1=CC=CC=C1C(=O)O) over 15 minutes."

**🤖 AI Agent:**
> The elution time is 12.3 minutes, with a capacity factor shift of 0.85 and an estimated peak width of 0.45 minutes.


## ❓ FAQ

**Q: What inputs are required for retention time prediction?**
You must provide the SMILES string of the compound, the column properties (stationary phase, length, particle size), the mobile phase details, and the operating temperature.

**Q: Can I compare different columns for my compounds?**
Yes, use the `compare_column_performance` tool to predict how switching between different column types will change the retention behavior for a set of compounds.

**Q: How does temperature affect the results?**
The model applies temperature as a scaling factor to the base retention time, accounting for the increased kinetic energy and decreased interaction strength at higher temperatures.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/retention-time-predictor](https://vinkius.com/ai-agent-connect/retention-time-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Retention Time Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `retention-time-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Retention Time Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "retention-time-predictor": {
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
