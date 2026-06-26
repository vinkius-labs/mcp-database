# Groove Quantize Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/groove-quantize-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate precise millisecond-based quantization grids, swing offsets, and latency compensation for DAWs.

## Description
The Groove Quantize Calculator is an essential tool for music producers working in Digital Audio Workstations (DAWs). It bridges the gap between musical tempo and absolute time by converting BPM into precise millisecond values. Use `calculate_note_durations` to find exact durations for standard, dotted, and triplet subdivisions. Determine the exact displacement needed for a specific feel with `calculate_swing_offset`. The server also provides `get_latency_recommendation` to help manage buffer sizes in high-tempo projects and `get_complete_rhythmic_map` for a full view of your rhythmic grid.


## Available Tools (4)
- **get_latency_recommendation**: Get recommended latency buffer based on BPM
- **calculate_note_durations**: g., "1/4", "1/8") to get millisecond values.

Calculate standard, dotted, and triplet durations for a subdivision
- **get_complete_rhythmic_map**: Generate a full rhythmic grid map
- **calculate_swing_offset**: Calculate millisecond displacement for swing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Groove Quantize Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the duration of a dotted 1/8th note at 140 BPM?"

**🤖 AI Agent:**
> At 140 BPM, a 1/8th note lasts approximately 214.29 ms, and its dotted version is approximately 321.43 ms.

---

**👤 You:**
> "Calculate the swing offset for 70% swing at 90 BPM."

**🤖 AI Agent:**
> For a 90 BPM project with a 70% swing target, the off-beat should be delayed by approximately 34.29 ms.

---

**👤 You:**
> "Show me a full rhythmic map for 128 BPM with 50% swing."

**🤖 AI Agent:**
> The complete rhythmic grid at 128 BPM (straight) includes: 1/4: 468.75ms, 1/8: 234.375ms, 1/16: 117.1875ms, etc.


## ❓ FAQ

**Q: How can I find the exact duration of a 1/16th note at 120 BPM?**
Use the `calculate_note_durations` tool. By providing 120 as the BPM and '1/16' as the subdivision, it will return the base duration in milliseconds.

**Q: How do I calculate the swing offset for a 66% swing feel?**
Use the `calculate_swing_offset` tool. Input your project's BPM and set the swing percentage to 66 to get the exact millisecond delay required for the off-beat.

**Q: Does this tool help with plugin latency?**
Yes. The `get_latency_recommendation` tool suggests appropriate buffer windows and provides warnings for high-tempo projects to help maintain rhythmic integrity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/groove-quantize-calculator](https://vinkius.com/mcp/groove-quantize-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Groove Quantize Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `groove-quantize-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Groove Quantize Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "groove-quantize-calculator": {
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
