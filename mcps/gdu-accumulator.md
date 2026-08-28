# GDU Accumulator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/gdu-accumulator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environmental-science](../categories/environmental-science.md)

Predict crop development stages and harvest timing using Growing Degree Units (GDU).

## Description
This MCP server provides tools to calculate Growing Degree Units (GDU), a critical metric for predicting crop phenology. By processing temperature data, it allows AI agents to track thermal accumulation from planting through maturity. Use `calculate_daily_gdu` to compute daily heat units, `get_cumulative_gdu` to sum heat over time, `predict_growth_stage` to identify current V-stages or R-stages, and `predict_maturity_and_harvest` to estimate physiological maturity dates and harvest windows.


## Available Tools (4)
- **calculate_daily_gdu**: Calculates the GDU value for a single day based on different mathematical methods
- **get_cumulative_gdu**: Calculates the total heat accumulated from the planting date up to a specific target date
- **predict_growth_stage**: Identifies which growth stage (V-stage or R-stage) the crop is likely in based on cumulative heat
- **predict_maturity_and_harvest**: Estimates the date when the crop will reach maturity and the subsequent harvest window


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GDU Accumulator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the GDU for a day with a max temp of 30°C, min temp of 15°C, base temp of 10°C, upper threshold of 35°C using the standard method."

**🤖 AI Agent:**
> The calculated GDU for that day is 12.5.

---

**👤 You:**
> "What growth stage is a corn crop in if it has accumulated 800 GDUs?"

**🤖 AI Agent:**
> Based on the provided thresholds, the corn is currently in the V12 stage.

---

**👤 You:**
> "Estimate the maturity date for a crop planted on May 1st that requires 1200 GDUs to mature, given a forecast of steady temperatures."

**🤖 AI Agent:**
> The crop is estimated to reach maturity on July 15th, with a harvest window starting July 18th.


## ❓ FAQ

**Q: What is a Growing Degree Unit (GDU)?**
A GDU is a measure of heat accumulation used to predict how quickly a crop will develop through its various growth stages.

**Q: How can I predict my harvest date?**
You can use the `predict_maturity_and_harvest` tool by providing the planting date, the required GDU for maturity, and a temperature forecast.

**Q: Does this tool account for environmental stress?**
Yes, the `calculate_daily_gdu` tool accepts a `stressFactor` to adjust heat accumulation for conditions like drought or waterlogging.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/gdu-accumulator](https://vinkius.com/ai-agent-connect/gdu-accumulator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GDU Accumulator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gdu-accumulator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GDU Accumulator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gdu-accumulator": {
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
