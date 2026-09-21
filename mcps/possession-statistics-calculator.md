# Possession Statistics Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/possession-statistics-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Calculate football possession percentages, average durations, and match timeline integrity.

## Description
This MCP server provides precise football possession analytics. It allows AI agents to process match data to determine home and away possession percentages, identify the longest continuous possession sequences, and calculate average possession durations. Use `calculate_possession_from_seconds` for quick totals or `calculate_possession_from_events` for detailed chronological analysis. It also includes `validate_match_timeline` to ensure all match periods are accounted for without gaps or overlaps, and `get_team_performance_comparison` to evaluate dominance between teams.


## Available Tools (4)
- **get_team_performance_comparison**: Provides a direct comparison of the two teams' possession metrics
- **calculate_possession_from_events**: Generates detailed statistics by processing a chronological list of possession changes
- **calculate_possession_from_seconds**: Calculates high-level possession metrics based on pre-aggregated time totals
- **validate_match_timeline**: Verifies if a sequence of possession events accurately covers the entirety of the match periods


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Possession Statistics Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate possession for a match with 5000s home, 4000s away, 500s disputed, and 9000s regulation time."

**🤖 AI Agent:**
> The home team had 55.56% possession, the away team had 44.44% possession, and disputed time was 5.56%. The conservation check is valid.

---

**👤 You:**
> "Compare the performance of a home team with 60% possession and an away team with 40% possession."

**🤖 AI Agent:**
> The home team is dominant with a possession difference of 20% and a dominance ratio of 1.5.

---

**👤 You:**
> "Check if these event durations [4500, 4500] cover a 90-minute match."

**🤖 AI Agent:**
> The total match time is 5400 seconds, and the total event time is 9000 seconds. The timeline is overlapping.


## ❓ FAQ

**Q: How do I calculate possession from a list of events?**
You can use the `calculate_possession_from_events` tool by providing a JSON string of the possession events along with the regulation and extra time durations.

**Q: Can I check if my match data has missing time gaps?**
Yes, the `validate_match_timeline` tool is designed to verify if the provided event durations cover the entire match period without gaps or overlaps.

**Q: How is team dominance determined?**
Dominance is calculated using `get_team_performance_comparison`, which compares the possession percentages of both teams to identify the dominant side and the dominance ratio.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/possession-statistics-calculator](https://vinkius.com/en/ai-agent-connect/possession-statistics-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Possession Statistics Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `possession-statistics-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Possession Statistics Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "possession-statistics-calculator": {
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
