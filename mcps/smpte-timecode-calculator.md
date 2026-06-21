# SMPTE Timecode Calculator MCP Server

Stop LLMs from melting down over base-60 math. Add, subtract, and convert video SMPTE timecodes natively.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/smpte-timecode-calculator)

## Overview
**Category:** developer-tools
**Tools Count:** 3

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


## Installation & Usage

To install and use the **SMPTE Timecode Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smpte-timecode-calculator](https://vinkius.com/mcp/smpte-timecode-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
