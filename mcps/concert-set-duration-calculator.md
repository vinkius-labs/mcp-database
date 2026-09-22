# Concert Set Duration Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/concert-set-duration-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate total setlist duration and manage performance time slots.

## Description
This MCP server helps concert organizers and performers manage performance timing. Use `get_total_set_duration` to find the cumulative length of a setlist, including optional gaps between songs. Use `validate_set_against_slot` to ensure your performance fits within venue time limits, or `calculate_ideal_buffer` to determine the perfect gap between songs to fill a specific time slot. It also provides detailed breakdowns via `get_setlist_summary`.


## Available Tools (4)
- **get_setlist_summary**: Provides a high-level breakdown of a setlist's composition and total length
- **validate_set_against_slot**: Checks if a proposed setlist fits within a specific allocated performance time slot
- **calculate_ideal_buffer**: Determines the maximum possible buffer time that can be placed between songs to perfectly fill an allocated time slot
- **get_total_set_duration**: Calculates the total time a setlist will take from start to finish


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concert Set Duration Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total duration for a set with songs lasting 180, 210, and 240 seconds, with a 10-second buffer between songs?"

**🤖 AI Agent:**
> The total set duration is 650 seconds (10 minutes and 50 seconds).

---

**👤 You:**
> "Will a setlist of songs lasting 300, 300, and 300 seconds fit in a 15-minute slot?"

**🤖 AI Agent:**
> Yes, the total duration is 900 seconds, which fits exactly into the 900-second (15-minute) slot.

---

**👤 You:**
> "Give me a summary for a set with songs of 120, 150, and 180 seconds."

**🤖 AI Agent:**
> The set consists of 3 songs with a total song time of 450 seconds.


## ❓ FAQ

**Q: How do I calculate the total time for my set?**
You can use the `get_total_set_duration` tool by providing a list of song durations in seconds and an optional buffer time for gaps between songs.

**Q: Can I check if my set fits in a 45-minute slot?**
Yes, use `validate_set_against_slot` by providing your song durations and the allocated time in seconds (e.g., 2700 for 45 minutes).

**Q: How do I find the best gap between songs to fill my time?**
The `calculate_ideal_buffer` tool will determine the maximum possible buffer time you can place between songs to perfectly fill your allocated time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/concert-set-duration-calculator](https://vinkius.com/en/ai-agent-connect/concert-set-duration-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concert Set Duration Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concert-set-duration-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concert Set Duration Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concert-set-duration-calculator": {
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
