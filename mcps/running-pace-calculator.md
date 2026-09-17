# Running Pace Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/running-pace-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

High-precision running pace, split times, and performance predictions.

## Description
A specialized utility for runners to perform precise calculations. Use `calculate_base_pace` to convert distance and time into pace, `get_split_times` to predict interval markers, `predict_equivalent_performance` to estimate times for different race distances, and `get_training_pace_targets` to define intensity zones for workouts.


## Available Tools (4)
- **calculate_base_pace**: 
- **get_split_times**: 
- **get_training_pace_targets**: 
- **predict_equivalent_performance**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Running Pace Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my pace for running 5km in 25 minutes?"

**🤖 AI Agent:**
> Your pace is 05:00 per km.

---

**👤 You:**
> "If I run a 10k in 50 minutes, what would my marathon time be?"

**🤖 AI Agent:**
> Your predicted marathon time is 03:52:15.

---

**👤 You:**
> "Give me my training zones for a 4:30 min/km pace."

**🤖 AI Agent:**
> Your training zones are: Easy (05:24), Marathon (04:30), Threshold (04:03), and Interval (03:36).


## ❓ FAQ

**Q: How can I calculate my pace?**
You can use the `calculate_base_pace` tool by providing your total distance and the time it took to complete the run.

**Q: Can I predict my marathon time from a 5k run?**
Yes, the `predict_equivalent_performance` tool uses physiological models to estimate your time for different distances.

**Q: How do I find my training zones?**
Use the `get_training_pace_targets` tool with your base race pace to receive a set of intensity-based training zones.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/running-pace-calculator](https://vinkius.com/en/ai-agent-connect/running-pace-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Running Pace Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `running-pace-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Running Pace Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "running-pace-calculator": {
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
