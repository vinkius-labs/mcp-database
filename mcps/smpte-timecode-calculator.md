# SMPTE Timecode Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/smpte-timecode-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Stop LLMs from melting down over base-60 math. Add, subtract, and convert video SMPTE timecodes natively.

## Description
LLMs are notoriously terrible at base-60 and base-30 math. If you ask an AI to add `00:01:23:14` to `00:02:45:21` at 29.97 drop-frame, the result is almost guaranteed to be a hallucination. This MCP fixes that for video automation pipelines.

### The Superpowers

- **Flawless Base-60 Math:** Perform exact frame-accurate addition and subtraction of SMPTE timecodes.
- **Drop-Frame Support:** Automatically accounts for NTSC 29.97 or 59.94 drop-frame logic.


## Available Tools (3)
- **frames_to_timecode**: Pass both timecode strings and the framerate, and receive the summed result.

Converts absolute frame counts into SMPTE formatted timecode strings
- **subtract_timecodes**: Pass the timecode and framerate.

Subtracts two SMPTE timecodes
- **add_timecodes**: Pass the frame count and the framerate (24, 25, 30, etc.).

Adds two SMPTE timecodes natively supporting drop-frame math


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SMPTE Timecode Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add the timecode `00:01:23:14` to `00:02:45:21` assuming a 29.97 drop-frame video format."

**🤖 AI Agent:**
> ✅ **SMPTE Calculation:** Base-60 addition resulted precisely in `00:04:09:05`.

---

**👤 You:**
> "Subtract exactly 30 frames from the starting timecode `00:01:00:00` at a standard 30fps rate."

**🤖 AI Agent:**
> ✅ **Frames Subtracted:** The resulting timecode is mathematically accurate: `00:00:59:00`.

---

**👤 You:**
> "Translate an absolute position of 1500 frames into a readable timecode string for a 25fps video."

**🤖 AI Agent:**
> ✅ **Timecode Formatted:** 1500 frames at 25fps maps perfectly to `00:01:00:00`.


## ❓ FAQ

**Q: Does it support drop-frame?**
Yes, pass the dropFrame boolean parameter for exact NTSC compliance.

**Q: What framerates are supported?**
All standard rates: 23.976, 24, 25, 29.97, 30, 50, 59.94, 60.

**Q: Can it convert frames to timecode?**
Yes, absolute frame counting to SMPTE string is supported.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smpte-timecode-calculator](https://vinkius.com/mcp/smpte-timecode-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SMPTE Timecode Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `smpte-timecode-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SMPTE Timecode Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "smpte-timecode-calculator": {
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
