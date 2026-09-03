# Concrete Curing Time Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-curing-time-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Predicts concrete curing duration, formwork removal, and loading readiness.

## Description
This MCP server provides precise technical calculations for concrete strength development. It uses the maturity method to determine how environmental factors like temperature and humidity affect hydration. Use `calculate_curing_duration` to find total curing time, `estimate_form_removal` to identify safe windows for stripping formwork from slabs or columns, and `estimate_loading_time` to predict when structural loads can be applied. It also offers `get_maturity_profile` for detailed strength evolution data.


## Available Tools (4)
- **estimate_form_removal**: Calculates the earliest safe moment to remove formwork
- **estimate_loading_time**: Predicts when the structure can safely support design loads
- **get_maturity_profile**: Provides a detailed look at how strength evolves over a specific timeframe
- **calculate_curing_duration**: Determines the total number of days required for the concrete to reach a target strength


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Curing Time Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many days will it take for Normal Weight concrete with Type I cement to reach 30 MPa at 25°C and 50% humidity?"

**🤖 AI Agent:**
> It will take 7 days for the concrete to reach 30 MPa under those conditions.

---

**👤 You:**
> "When can I safely remove the forms from a concrete column using Type III cement at 20°C and 60% humidity?"

**🤖 AI Agent:**
> The formwork for the column can be safely removed in 48 hours.

---

**👤 You:**
> "Show me the strength profile for High Performance concrete over 14 days at 22°C and 55% humidity."

**🤖 AI Agent:**
> The strength profile shows a rapid increase in the first 3 days, reaching 15 MPa, followed by a steady climb to 35 MPa by day 14.


## ❓ FAQ

**Q: How does temperature affect the results?**
Temperature is a primary driver of the maturity index. Higher temperatures accelerate the chemical hydration process, while lower temperatures slow it down.

**Q: Can I account for chemical additives?**
Yes, you can include admixtures like accelerators or retarders in the tool inputs to adjust the predicted strength gain rate.

**Q: What is the difference between form removal and loading time?**
Form removal time is when the concrete can support its own weight and the forms, whereas loading time is when it can support the actual design loads.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-curing-time-predictor](https://vinkius.com/ai-agent-connect/concrete-curing-time-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Curing Time Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-curing-time-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Curing Time Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-curing-time-predictor": {
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
