# Running Splits Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/running-splits-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Decompose target times and distances into precise pacing segments and strategies.

## Description
This MCP server provides specialized tools for runners to manage their pacing. Use `calculate_splits_and_progress` to get a full breakdown of split times and cumulative progress. Plan an acceleration strategy using `calculate_negative_split_strategy` to finish stronger. You can also use `compare_pace_targets` to check if you are on track during a run, or `get_split_summary` to evaluate your performance after a workout.


## Available Tools (4)
- **calculate_negative_split_strategy**: Generates a pacing plan where the runner progressively accelerates throughout the workout
- **calculate_splits_and_progress**: Provides a complete breakdown of a workout including individual split times, cumulative elapsed time, and required pace per segment
- **compare_pace_targets**: Compares a user's current average pace against a theoretical target pace to determine if they are ahead or behind schedule
- **get_split_summary**: Provides a high-level summary of a completed workout to quickly assess performance against a goal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Running Splits Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to run 10km in 50 minutes. Can you give me a breakdown of my splits every 1km?"

**🤖 AI Agent:**
> To complete 10km in 50 minutes, your target pace is 5:00 per km. Your splits will be: 1km at 5:00, 2km at 10:00, 3km at 15:00, 4km at 20:00, 5km at 25:00, 6km at 30:00, 7km at 35:00, 8km at 40:00, 9km at 45:00, and 10km at 50:00.

---

**👤 You:**
> "I've run 5km in 25 minutes. I want to finish 10km in 52 minutes. Am I on track?"

**🤖 AI Agent:**
> Your target pace for 10km in 52 minutes is 5:12 per km. Since you have covered 5km in 25 minutes (a pace of 5:00 per km), you are currently ahead of schedule.

---

**👤 You:**
> "Help me plan a negative split for a 5km run in 25 minutes, with an acceleration factor of 1.05."

**🤖 AI Agent:**
> For a 5km run in 25 minutes with a 1.05 acceleration factor, your segments will progressively speed up. Your splits will be approximately: 1km at 5:18, 2km at 5:10, 3km at 5:02, 4km at 4:54, and 5km at 4:46.


## ❓ FAQ

**Q: How can I plan a race with a faster finish?**
You can use the `calculate_negative_split_strategy` tool to generate a plan where each segment is progressively faster than the last.

**Q: Can I check if I am running too slow during my workout?**
Yes, use `compare_pace_targets` to compare your current elapsed time and distance against your target pace to see if you are ahead or behind.

**Q: What kind of breakdown can I get for my run?**
The `calculate_splits_and_progress` tool provides split times, cumulative elapsed time, and the required pace for every segment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/running-splits-calculator](https://vinkius.com/en/ai-agent-connect/running-splits-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Running Splits Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `running-splits-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Running Splits Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "running-splits-calculator": {
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
