# EMOM Timer Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/emom-timer-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate structured Every Minute on the Minute (EMOM) workout protocols with precise timing and volume calculations.

## Description
This MCP server provides specialized tools for designing high-intensity EMOM (Every Minute on the Minute) training sessions. It allows AI agents to build complete workout plans using `generate_emom_protocol`, predict total workload with `calculate_volume_projection`, and analyze difficulty shifts via `evaluate_intensity_scaling`. You can also use `get_timing_breakdown` to see the exact work and rest windows for any interval. It is designed to help athletes and coaches structure training with mathematical precision.


## Available Tools (4)
- **calculate_volume_projection**: Predicts the total workload for different workout lengths
- **evaluate_intensity_scaling**: Analyzes how the difficulty changes throughout the protocol based on the chosen progression
- **generate_emom_protocol**: Creates a complete, structured EMOM workout plan based on user-defined exercises and duration
- **get_timing_breakdown**: Provides a granular second-by-second breakdown of a single EMOM interval


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EMOM Timer Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 10-minute EMOM protocol for Kettlebell Swings with 15 reps per round using a fixed work strategy."

**🤖 AI Agent:**
> Your 10-minute EMOM protocol for Kettlebell Swings is ready. You will perform 15 reps each minute for 10 rounds, totaling 150 repetitions. Each minute consists of a work window and a rest window.

---

**👤 You:**
> "How many total reps will I do if I perform 10 burpees per minute for 20 minutes?"

**🤖 AI Agent:**
> You will complete a total volume of 200 repetitions.

---

**👤 You:**
> "Show me the timing breakdown for a 40-second work window."

**🤖 AI Agent:**
> For a 40-second work window, you will have 40 seconds of work and 20 seconds of rest within the 60-second interval.


## ❓ FAQ

**Q: How do I create a full workout plan?**
You can use the `generate_emom_protocol` tool by providing the exercise name, repetitions per round, total duration, and your preferred rest strategy.

**Q: Can I predict the total repetitions for a longer workout?**
Yes, use the `calculate_volume_projection` tool to estimate the total workload based on your repetitions per minute and the desired duration.

**Q: How does the tool handle rest periods?**
The tool calculates the rest window as the remaining time in the sixty-second interval after the work window is completed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/emom-timer-builder](https://vinkius.com/en/ai-agent-connect/emom-timer-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EMOM Timer Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emom-timer-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EMOM Timer Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emom-timer-builder": {
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
