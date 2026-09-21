# Sound Bath Frequency Selector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sound-bath-frequency-selector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate optimized sound bath session plans by matching therapeutic frequencies to goals and instruments.

## Description
This MCP server provides practitioners with the tools to design structured sound healing sessions. By using `plan_sound_bath`, you can generate a complete sequence of instruments, frequencies, and durations tailored to specific therapeutic intentions like grounding or clarity. The server also includes `validate_instrument_capability` to ensure your tools match the required frequency ranges, and `calculate_tone_timing` to adjust resonance based on participant count. It bridges the gap between therapeutic sound principles and practical session planning.


## Available Tools (4)
- **get_goal_frequency_mapping**: Retrieves the target frequency spectrum and required instrument types for a given therapeutic goal
- **calculate_tone_timing**: Determines how long each tone should be held to ensure effective resonance for the group
- **plan_sound_bath**: Generates a complete, structured sound bath session plan based on a specific therapeutic goal and available resources
- **validate_instrument_capability**: Checks if a specific instrument is capable of producing a specific frequency range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sound Bath Frequency Selector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a grounding sound bath for 10 people using large gongs and deep singing bowls."

**🤖 AI Agent:**
> Your grounding session plan is ready. It will feature a 45-minute sequence starting with low-frequency gongs to establish stability, followed by deep singing bowls for resonance, totaling 45 minutes.

---

**👤 You:**
> "Can a small tuning fork produce low frequencies?"

**🤖 AI Agent:**
> No, a small tuning fork is typically only capable of producing high-frequency ranges.

---

**👤 You:**
> "What frequencies are needed for mental clarity?"

**🤖 AI Agent:**
> Mental clarity sessions require mid-to-high frequency instruments to assist in removing cognitive fog.


## ❓ FAQ

**Q: How do I create a full session plan?**
Use the `plan_sound_bath` tool by providing your session goal, the list of instruments you have, and the number of participants.

**Q: Can I check if my singing bowls are suitable for a specific goal?**
Yes, you can use `validate_instrument_capability` to check if an instrument can produce the required low, mid, or high frequency ranges.

**Q: Does the session duration change with group size?**
Yes, the `calculate_tone_timing` tool automatically adjusts tone durations to ensure effective resonance for larger groups.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sound-bath-frequency-selector](https://vinkius.com/en/ai-agent-connect/sound-bath-frequency-selector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sound Bath Frequency Selector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sound-bath-frequency-selector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sound Bath Frequency Selector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sound-bath-frequency-selector": {
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
