# Deload Week Inserter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deload-week-inserter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automatically integrate recovery weeks into your training blocks by scaling weights and volume.

## Description
The Deload Week Inserter MCP server allows you to transform a standard training routine into a complete, periodized training block. By using the `apply_deload_logic` tool, you can specify an interval for recovery and a reduction factor to automatically scale down intensity and volume during deload weeks. It also provides tools like `validate_deload_training_config` to ensure your parameters are mathematically sound and `count_recovery_occurrences` to predict how many recovery periods will occur in your block.


## Available Tools (3)
- **apply_deload_logic**: Generates a modified training schedule with recovery weeks
- **count_recovery_occurrences**: Counts how many recovery weeks occur in a block
- **validate_deload_training_config**: Ensures deload settings are mathematically sound


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deload Week Inserter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Apply a 60% deload every 4 weeks to this routine: [{"week": 1, "exercises": []}, {"week": 2, "exercises": []}, {"week": 3, "exercises": []}, {"week": 4, "exercises": [{"name": "Squat", "weight": 100, "volume": 5}]}]"

**🤖 AI Agent:**
> [{"week": 1, "exercises": []}, {"week": 2, "exercises": []}, {"week": 3, "exercises": []}, {"week": 4, "exercises": [{"name": "Squat", "weight": 60, "volume": 3}]}]

---

**👤 You:**
> "Is a deload percentage of 1.2 valid?"

**🤖 AI Agent:**
> No, the configuration is invalid because the reduction percentage must be between 0 and 1 to ensure a decrease in workload.

---

**👤 You:**
> "How many deloads will occur in a 12-week block with a 4-week interval?"

**🤖 AI Agent:**
> There will be 3 recovery weeks integrated into your training block.


## ❓ FAQ

**Q: How does the deload logic work?**
The `apply_deload_logic` tool iterates through your weekly routine. When it reaches a week number divisible by your specified interval, it multiplies all weights and volumes in that week by your reduction factor.

**Q: Can I validate my deload settings before applying them?**
Yes, you can use the `validate_deload_training_config` tool to check if your recovery interval and reduction percentage are appropriate for standard training practices.

**Q: What is a deload week?**
A delog week is a scheduled period of reduced training intensity and volume to facilitate physical recovery.

**Q: How can I calculate the number of recovery periods?**
Use the `count_recovery_occurrences` tool by providing the total duration of your training block and the frequency interval for deloads.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deload-week-inserter](https://vinkius.com/mcp/deload-week-inserter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deload Week Inserter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `deload-week-inserter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deload Week Inserter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deload-week-inserter": {
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
