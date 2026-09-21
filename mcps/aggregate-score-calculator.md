# Aggregate Score Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/aggregate-score-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate aggregate winners and tiebreak requirements for two-legged football ties.

## Description
This MCP server provides specialized tools for football analysts and fans to determine the outcome of two-legged ties. It calculates total goals, identifies the aggregate winner, and determines if a tie requires extra time or a penalty shootout. Use `calculate_tie_result` to get a full overview of the tie status, or `evaluate_tiebreak_necessity` to check if the match is level and needs further play.


## Available Tools (4)
- **calculate_tie_result**: Determines the outcome of a two-legged tie including total goals, winner, and tiebreak requirements
- **check_shootout_eligibility**: Validates if a tie is in a state where a penalty shootout is the logical next step
- **evaluate_tiebreak_necessity**: Determines if a tie requires additional play (extra time or penalties) based on current scores
- **get_team_aggregate_summary**: Provides a simplified summary of one specific team's performance across the tie


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aggregate Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Team One scored 2 in the first leg and 1 in the second. Team Two scored 1 in the first leg and 1 in the second. What is the result?"

**🤖 AI Agent:**
> Team One is the aggregate winner with 3 total goals compared to Team Two's 2 total goals.

---

**👤 You:**
> "The aggregate score is 2-2 after both legs. Has extra time been played?"

**🤖 AI Agent:**
> If extra time has not been played, the next step is Extra Time. If extra time has been played, the next step is a Penalty Shootout.

---

**👤 You:**
> "Team One has 3 goals total and Team Two has 3 goals total. They just finished extra time. What happens next?"

**🤖 AI Agent:**
> The tie is level and the required next step is a Penalty Shootout.


## ❓ FAQ

**Q: How does the tool handle penalty shootouts?**
The tool treats penalty shootout results separately. Shootout goals are used to identify the winner but are not added to the aggregate goal count.

**Q: Can I check if a match needs extra time?**
Yes, you can use `evaluate_tiebreak_necessity` to determine if the current aggregate score requires extra time or a penalty shootout.

**Q: What information is returned for a tie result?**
The `calculate_tie_result` tool returns total goals for both teams, the aggregate winner, the tie status, and the required next tiebreak procedure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/aggregate-score-calculator](https://vinkius.com/en/ai-agent-connect/aggregate-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aggregate Score Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aggregate-score-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aggregate Score Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aggregate-score-calculator": {
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
