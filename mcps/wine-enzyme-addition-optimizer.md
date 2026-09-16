# Wine Enzyme Addition Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-enzyme-addition-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Optimize enzyme dosage and contact time for grape must extraction and clarification.

## Description
This MCP server provides specialized tools for winemakers to optimize enzyme additions during the extraction and clarification processes. By analyzing grape variety cell wall structures, temperature, and pH levels, the server calculates precise dosage rates and contact times. Use `calculate_optimal_dosage` to find the ideal amount of pectinase, cellulase, or protease for a specific must. You can also use `evaluate_extraction_efficiency` to predict improvements in target compound extraction, `compare_enzyme_strategies` to select the best enzyme for color extraction or clarification, and `simulate_native_activity_impact` to account for indigenous enzymatic activity in different grape varieties.


## Available Tools (4)
- **calculate_optimal_dosage**: Determines the ideal amount of enzyme to add to a specific must
- **evaluate_extraction_efficiency**: Predicts how much the extraction of target compounds will improve
- **simulate_native_activity_impact**: Estimates how much natural enzymes in a variety will reduce the need for added enzymes
- **compare_enzyme_strategies**: Compares different enzyme types to find the best approach


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Enzyme Addition Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the optimal dose of pectinase for Cabernet Sauvignon at 20 degrees Celsius and pH 3.5?"

**🤖 AI Agent:**
> The optimal dose rate for pectinase is 0.05 L/h with a predicted extraction improvement of 15% over a 4-hour contact time.

---

**👤 You:**
> "Compare enzyme strategies for clarification in Merlot at 18 degrees Celsius and pH 3.2."

**🤖 AI Agent:**
> For clarification in Merlot, protease is the best enzyme type, requiring a dose of 0.03 L/h with a 3-hour contact time.

---

**👤 You:**
> "Will adding 0.04 L/h of cellulase to Pinot Noir at 22 degrees Celsius improve extraction?"

**🤖 AI Agent:**
> Yes, the predicted improvement is 12% with an efficiency rating of 'Optimal'.


## ❓ FAQ

**Q: How do I determine the best enzyme for color extraction?**
You can use the `compare_enzyme_strategies` tool with the target goal set to 'color_extraction' to identify whether pectinase or cellulase is most effective for your specific grape variety.

**Q: Can I account for the natural enzymes already present in my grapes?**
Yes, the `simulate_native_activity_impact` tool estimates how much the natural enzymes in a variety will reduce the required dose of added enzymes.

**Q: How does temperature affect the enzyme dosage?**
Temperature is a critical factor in enzyme kinetics. The `calculate_optimal_dosage` tool automatically adjusts the recommended dose and contact time based on the current temperature of the must.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-enzyme-addition-optimizer](https://vinkius.com/en/ai-agent-connect/wine-enzyme-addition-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Enzyme Addition Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-enzyme-addition-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Enzyme Addition Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-enzyme-addition-optimizer": {
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
