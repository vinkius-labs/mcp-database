# Substitution Window Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/substitution-window-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [compliance](../categories/compliance.md)

A regulatory compliance engine for monitoring football substitution limits, windows, and bench capacity.

## Description
This MCP server provides a regulatory compliance engine for monitoring football substitution limits, window constraints, and bench capacity during matches. It allows AI agents to track remaining player substitutions and available windows using `query_current_status`. Coaches and analysts can record specific events with `register_substitution` to ensure compliance with competition rules. The engine also supports checking phase transitions via `validate_window_transition` and monitoring remaining bench depth with `get_bench_availability`.


## Available Tools (4)
- **get_bench_availability**: Checks how many players are still available on the bench to be substituted
- **query_current_status**: Retrieves the current remaining substitution allowance and state for a specific team
- **register_substitution**: Records a substitution event and validates it against all competition rules
- **validate_window_transition**: Checks if a team can open a new substitution window based on the current match phase


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Substitution Window Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current substitution status for team 'T123'?"

**🤖 AI Agent:**
> Team T123 has 2 player substitutions and 1 window remaining. 3 players from the bench have already entered the pitch.

---

**👤 You:**
> "Register a substitution for team 'T123': player 'P99' in for player 'P44' at minute 65. This is the start of a new window."

**🤖 AI Agent:**
> Substitution successful. Remaining player substitutions: 1. Remaining windows: 0.

---

**👤 You:**
> "Can team 'T123' open a new window during the half-time phase?"

**🤖 AI Agent:**
> Yes, the transition to half-time allows for a new substitution window.


## ❓ FAQ

**Q: How do I check if a team has any substitutions left?**
You can use the `query_current_status` tool to retrieve the remaining player substitutions and available windows for a specific team.

**Q: Can I record a substitution that happens at half-time?**
Yes, you can use `register_substitution` to record the event. The engine will validate if the substitution is permitted during the current match phase.

**Q: How do I know if the bench is full?**
Use the `get_bench_availability` tool to see how many players are still available on the bench for a given team.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/substitution-window-tracker](https://vinkius.com/en/ai-agent-connect/substitution-window-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Substitution Window Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `substitution-window-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Substitution Window Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "substitution-window-tracker": {
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
