# Swimming Rest & Training Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/swimming-rest-training-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate total rest, set duration, and training intensity for swim sets.

## Description
This MCP server provides essential tools for swim coaches and athletes to manage training volume and intensity. By connecting to Vinkius Edge, AI agents can use tools like `get_total_rest` to calculate cumulative rest, `get_set_duration` to find total elapsed time, `get_rest_ratio` to evaluate intensity, and `get_training_density` to measure work relative to pool time. It helps in precisely planning training blocks and monitoring physiological load.


## Available Tools (4)
- **get_rest_ratio**: Calculates the ratio of rest time to active swimming time to evaluate training intensity
- **get_set_duration**: Determines the total time elapsed for a set, including both swimming time and rest time
- **get_total_rest**: Calculates the total amount of rest time for a specific set of repetitions
- **get_training_density**: Calculates how much "work" is done relative to the total time spent in the pool


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Swimming Rest & Training Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total rest time for 10 repetitions with a 30 second rest interval?"

**🤖 AI Agent:**
> The total rest time for 10 repetitions with a 30 second rest interval is 300 seconds.

---

**👤 You:**
> "Calculate the total duration for a set of 5 reps, where each swim is 60 seconds and rest is 45 seconds."

**🤖 AI Agent:**
> The total duration for the set is 525 seconds.

---

**👤 You:**
> "What is the rest to swim ratio if I swim for 50 seconds and rest for 25 seconds?"

**🤖 AI Agent:**
> The rest to swim ratio is 0.5.


## ❓ FAQ

**Q: How do I use this with my AI assistant?**
Simply connect to Vinkius Edge using your Connection Token. Once connected, you can ask your AI assistant in Cursor, Claude Desktop, or VS Code to calculate rest times or training density using the provided tools.

**Q: What can `get_total_rest` calculate?**
The `get_total_rest` tool calculates the cumulative rest time by multiplying the duration of a single rest interval by the number of repetitions performed.

**Q: Can I calculate training density?**
Yes, you can use `get_training_density` to find the percentage of the total set time spent actively swimming.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/swimming-rest-training-calculator](https://vinkius.com/en/ai-agent-connect/swimming-rest-training-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Swimming Rest & Training Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `swimming-rest-training-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Swimming Rest & Training Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "swimming-rest-training-calculator": {
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
