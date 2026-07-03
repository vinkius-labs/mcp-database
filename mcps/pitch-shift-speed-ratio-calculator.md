# Pitch Shift Speed Ratio Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pitch-shift-speed-ratio-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate playback speed multipliers, adjusted durations, and new BPM for pitch shifting via varispeed.

## Description
The Pitch Shift Speed Ratio Calculator is a specialized utility for audio producers and DJs. It allows you to determine the exact playback speed multiplier, new duration, and adjusted BPM required to achieve specific pitch changes using the varispeed method. By using tools like `get_speed_rate`, `transform_duration`, `transform_bpm`, and `reverse_semitone_lookup`, you can quickly match the key of two audio loops by speeding up or slowing down playback without needing complex digital signal processing.


## Available Tools (4)
- **get_speed_rate**: Use when you know how many semitones to shift.

Determines the necessary playback speed multiplier for a target pitch change
- **reverse_semitone_lookup**: Use when you know the desired ratio.

Determines the number of semitones needed to reach a specific target speed ratio
- **transform_bpm**: Use when you have original BPM and a ratio.

Calculates the new tempo (BPM) for a musical loop after speed adjustment
- **transform_duration**: Use when you have original length and a ratio.

Calculates the new duration of an audio clip after speed adjustment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pitch Shift Speed Ratio Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to shift an audio loop up by 2 semitones. What speed ratio do I need?"

**🤖 AI Agent:**
> The required playback speed multiplier is approximately 1.122.

---

**👤 You:**
> "If my original track is 120 BPM and I apply a ratio of 0.9, what will the new BPM be?"

**🤖 AI Agent:**
> The new tempo will be 108 BPM.

---

**👤 You:**
> "How long will a 3-minute (180 seconds) clip be if I use a speed ratio of 1.5?"

**🤖 AI Agent:**
> The new duration will be 120 seconds.


## ❓ FAQ

**Q: What is the varispeed method?**
The varispeed method involves changing the playback speed of an audio file to alter its pitch. This process naturally changes both the tempo (BPM) and the duration of the clip.

**Q: How can I find the speed multiplier for a specific semitone shift?**
You can use the `get_speed_rate` tool. Simply provide the number of semitones you want to shift (positive for higher pitch, negative for lower), and it will return the required ratio.

**Q: Can I calculate the new BPM after a speed change?**
Yes, use the `transform_bpm` tool. By providing your original BPM and the playback ratio, you will get the new tempo.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pitch-shift-speed-ratio-calculator](https://vinkius.com/mcp/pitch-shift-speed-ratio-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pitch Shift Speed Ratio Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pitch-shift-speed-ratio-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pitch Shift Speed Ratio Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pitch-shift-speed-ratio-calculator": {
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
