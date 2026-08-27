# Wine Tannin Extraction Kinetics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-tannin-extraction-kinetics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predict tannin extraction from seeds and skins during fermentation.

## Description
This MCP server provides enologists with predictive modeling for tannin extraction during fermentation. It uses a biphasic model to simulate how tannins are released from grape skins and seeds. Users can use `simulate_extraction_kinetics` to predict tannin concentrations over time, `calculate_optimal_maceration` to find the ideal contact time for a specific sensory profile, `evaluate_varietal_impact` to compare different maturity levels, and `predict_alcohol_influence` to see how rising ethanol affects extraction speed.


## Available Tools (4)
- **calculate_optimal_maceration**: Identify the best time to stop skin contact to achieve a target sensory profile
- **evaluate_varietal_impact**: Compare how different grape maturities will affect the final tannin profile
- **predict_alcohol_influence**: Determine how rising alcohol levels will alter the extraction speed of tannins
- **simulate_extraction_kinetics**: Predict the concentration of tannins over a specific period of time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Tannin Extraction Kinetics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the tannin concentration for a fermentation at 25°C with a seed browning index of 5 over 100 hours."

**🤖 AI Agent:**
> At 25°C and a browning index of 5, the predicted skin tannin concentration is 0.45 g/L and the seed tannin concentration is 0.22 g/L after 100 hours.

---

**👤 You:**
> "What is the optimal maceration time for a target astringency of 0.3 and a skin-to-seed ratio of 2.5?"

**🤖 AI Agent:**
> The optimal contact time to achieve an astringency of 0.3 and a 2.5 tannin ratio is 72 hours.

---

**👤 You:**
> "How will an alcohol evolution rate of 0.05% per hour affect the extraction?"

**🤖 AI Agent:**
> An alcohol evolution rate of 0.05% per hour results in an extraction acceleration factor of 1.12 for the predicted period.


## ❓ FAQ

**Q: How does the biphasic model work?**
The model simulates two stages: a fast initial extraction from grape skins and a slower, more prolonged release from the seeds.

**Q: Can I predict the effect of temperature on extraction?**
Yes, by using `simulate_extraction_kinetics`, you can input different temperature values to see how they accelerate or decelerate the extraction process.

**Q: How do I find the best time to stop skin contact?**
Use the `calculate_optimal_maceration` tool. You provide your target astringency and tannin ratio, and it identifies the optimal contact hours.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-tannin-extraction-kinetics](https://vinkius.com/ai-agent-connect/wine-tannin-extraction-kinetics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Tannin Extraction Kinetics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-tannin-extraction-kinetics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Tannin Extraction Kinetics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-tannin-extraction-kinetics": {
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
