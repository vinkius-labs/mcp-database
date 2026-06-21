# SMPTE Timecode Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/smpte-timecode-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/smpte-timecode-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/smpte-timecode-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Stop LLMs from melting down over base-60 math. Add, subtract, and convert video SMPTE timecodes natively.

## Description
LLMs are notoriously terrible at base-60 and base-30 math. If you ask an AI to add `00:01:23:14` to `00:02:45:21` at 29.97 drop-frame, the result is almost guaranteed to be a hallucination. This MCP fixes that for video automation pipelines.

### The Superpowers

- **Flawless Base-60 Math:** Perform exact frame-accurate addition and subtraction of SMPTE timecodes.
- **Drop-Frame Support:** Automatically accounts for NTSC 29.97 or 59.94 drop-frame logic.


## Available Tools
- **add_timecodes**: Pass the frame count and the framerate (24, 25, 30, etc.).

Adds two SMPTE timecodes natively supporting drop-frame math
- **frames_to_timecode**: Pass both timecode strings and the framerate, and receive the summed result.

Converts absolute frame counts into SMPTE formatted timecode strings
- **subtract_timecodes**: Pass the timecode and framerate.

Subtracts two SMPTE timecodes


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


## Installation & Usage

To install and use the **SMPTE Timecode Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smpte-timecode-calculator](https://vinkius.com/mcp/smpte-timecode-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
