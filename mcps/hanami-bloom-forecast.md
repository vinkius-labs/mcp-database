# Hanami Bloom Forecast MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/hanami-bloom-forecast)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predict Japanese cherry blossom (Sakura) bloom dates using thermal degree day accumulation.

## Description
This MCP server provides a deterministic forecasting engine for Japanese cherry blossom (Sakura) bloom stages. By analyzing accumulated thermal energy above a biological threshold, it calculates the exact dates for initial bloom and full bloom. Use `calculate_bloom_forecast` to predict bloom windows, `get_thermal_accumulation_summary` to view daily heat accumulation, and `validate_bloom_parameters` to ensure biological constants are within realistic ranges.


## Available Tools (3)
- **calculate_bloom_forecast**: 
- **get_thermal_accumulation_summary**: Provides heat accumulation breakdown
- **validate_bloom_parameters**: Validates biological constants


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hanami Bloom Forecast** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the bloom date for a Somei Yoshino cherry tree with a base temperature of 5°C and 350 required degree days, given these temperatures: [2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40]"

**🤖 AI Agent:**
> The predicted bloom date is April 12th, 2024, with a full bloom expected on April 19th, 2024.

---

**👤 You:**
> "Show me the thermal accumulation summary for temperatures [5, 5, 10, 10, 15, 15] with a base temperature of 5°C."

**🤖 AI Agent:**
> The total accumulated degree days is 30. The daily accumulation was 0, 0, 5, 5, 10, 10.

---

**👤 You:**
> "Is a base temperature of -10°C valid for Sakura bloom forecasting?"

**🤖 AI Agent:**
> No, a base temperature of -10°C is outside the standard biological range for these calculations.


## ❓ FAQ

**Q: How does the bloom prediction work?**
The engine uses the Degree Day method, calculating the sum of daily temperatures that exceed a specific base temperature threshold to predict when the Sakura will bloom.

**Q: What is the base temperature used for?**
The base temperature is the biological threshold below which no thermal accumulation occurs for the cherry tree's growth processes.

**Q: Can I validate my input parameters?**
Yes, you can use the `validate_bloom_parameters` tool to check if your base temperature and required degree days are within realistic biological bounds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/hanami-bloom-forecast](https://vinkius.com/ai-agent-connect/hanami-bloom-forecast)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hanami Bloom Forecast** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hanami-bloom-forecast` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hanami Bloom Forecast** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hanami-bloom-forecast": {
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
