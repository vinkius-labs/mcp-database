# Running Race Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/running-race-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Predict race performance and generate segmented pacing strategies using the Riegel model.

## Description
The Running Race Predictor MCP server connects AI agents to advanced endurance modeling. By providing a recent race result, you can use `predict_race_times` to estimate your performance across standard distances like 5K, 10K, and Marathons using the Riegel fatigue model. For upcoming goals, use `generate_segment_strategy` to create actionable pacing plans (Even Split, Negative Split, or Conservative Start) broken down by race segments. You can also use `validate_race_input` to ensure all your distance measurements are correctly normalized to meters before processing.


## Available Tools (3)
- **predict_race_times**: Predicts race times for standard distances
- **generate_segment_strategy**: Generates a segmented pacing strategy
- **validate_race_input**: Validates and normalizes race distance input


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Running Race Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I ran a 5K in 25 minutes. What can I expect for a Marathon?"

**🤖 AI Agent:**
> Based on your 5K time of 25:00, your predicted Marathon time is approximately 3:56:42 with a pace of 5:36 min/km.

---

**👤 You:**
> "Generate a pacing strategy for a 10K race with a goal time of 50 minutes using a negative split approach."

**🤖 AI Agent:**
> For your 10,000m goal of 50:00, here is your strategy:
- Segment 1 (Start): 3,333m at 5:05 min/km
- Segment 2 (Middle): 3,333m at 5:00 min/km
- Segment 3 (Finish): 3,334m at 4:55 min/km

---

**👤 You:**
> "Is 10 miles a valid distance input?"

**🤖 AI Agent:**
> Yes, 10 miles is a valid input. It has been normalized to 16093.4 meters.


## ❓ FAQ

**Q: How accurate are the race predictions?**
Predictions use the Riegel model, which is highly effective for standard distances. For ultra-endurance distances exceeding a marathon, the system applies an adjusted fatigue exponent to maintain accuracy.

**Q: What pacing strategies are available?**
You can choose from `EVEN_SPLIT` for constant speed, `NEGATIVE_SPLIT` to finish faster than you started, or `CONSERVATIVE_START` to conserve energy early in the race.

**Q: Can I use my own distance measurements?**
Yes. You can provide distances in meters, kilometers, or miles. The `validate_race_input` tool will automatically normalize them to meters for precise calculation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/running-race-predictor](https://vinkius.com/mcp/running-race-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Running Race Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `running-race-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Running Race Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "running-race-predictor": {
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
