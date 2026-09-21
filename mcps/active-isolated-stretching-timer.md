# Active Isolated Stretching Timer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/active-isolated-stretching-timer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

A timing engine for the Aaron Mattes Active Isolated Stretching (AIS) protocol.

## Description
This MCP server provides a specialized timing engine for the Aaron Mattes Active Isolated Stretching (AIS) protocol. It helps users manage the precise timing required to avoid the stretch reflex. Use `calculate_stretch_cycle` to determine the timing for a single repetition, `calculate_set_metrics` to plan the total duration of a set, `get_antagonist_guidance` to identify the muscle needed for reciprocal inhibition, and `validate_protocol_safety` to ensure the requested repetitions and assistance levels are appropriate for the target muscle group.


## Available Tools (4)
- **calculate_set_metrics**: Calculates the cumulative timing and repetition data for a complete set of stretches
- **calculate_stretch_cycle**: Determines the timing and structure of a single repetition within a stretching set
- **get_antagonist_guidance**: Identifies which muscle must be activated to facilitate the stretch for the target muscle
- **validate_protocol_safety**: Evaluates if the requested parameters are appropriate for a specific muscle group


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Active Isolated Stretching Timer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long should I hold a stretch for the hamstrings with moderate assistance?"

**🤖 AI Agent:**
> For a hamstring stretch with moderate assistance, the hold duration is 1.5 seconds.

---

**👤 You:**
> "Calculate the total time for 10 reps of a quadriceps stretch with no assistance."

**🤖 AI Agent:**
> The total time for 10 repetitions of the quadriceps stretch with no assistance is 45 seconds.

---

**👤 You:**
> "Which muscle should I activate to stretch my biceps?"

**🤖 AI Agent:**
> To stretch your biceps, you should actively contract your triceps.


## ❓ FAQ

**Q: What is the purpose of the AIS protocol?**
The Active Isolated Stretching (AIS) protocol is designed to increase range of motion and reduce muscle tension by using short, controlled movements that avoid triggering the stretch reflex.

**Q: How do I know which muscle to contract during a stretch?**
You can use the `get_antagonist_guidance` tool to identify the specific antagonist muscle that must be activated to facilitate the stretch through reciprocal inhibition.

**Q: Can I check if my stretching routine is safe?**
Yes, the `validate_protocol_safety` tool evaluates if your chosen repetitions and assistance levels are appropriate for the specific muscle group you are targeting.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/active-isolated-stretching-timer](https://vinkius.com/en/ai-agent-connect/active-isolated-stretching-timer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Active Isolated Stretching Timer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `active-isolated-stretching-timer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Active Isolated Stretching Timer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "active-isolated-stretching-timer": {
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
