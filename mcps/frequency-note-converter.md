# Frequency & Note Converter MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/frequency-note-converter)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/frequency-note-converter-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/frequency-note-converter-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Convert between musical frequencies and notes with precision.

## Description
A high-precision utility for musicians and audio engineers to bridge the gap between Hertz (Hz) and musical pitch. This MCP server provides tools like `frequency_to_note` to identify notes from frequencies, `note_to_frequency` for exact frequency calculation, `calculate_harmonics` for harmonic series generation, and `get_pitch_depth` to measure distance from the A0 baseline. Supports both 440Hz and 432Hz tuning standards.


## Available Tools
- **calculate_harmonics**: Calculate the fundamental harmonic series for a frequency
- **hz_to_note**: Convert frequency in Hz to the nearest musical note
- **note_to_hz**: Convert a musical note and octave to frequency in Hz
- **get_pitch_depth**: Calculate how high a frequency is above the A0 baseline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Frequency & Note Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What note is 440Hz in the standard tuning?"

**🤖 AI Agent:**
> 440Hz corresponds to the note A4.

---

**👤 You:**
> "Convert C4 to frequency using 432Hz tuning."

**🤖 AI Agent:**
> The frequency for C4 in 432Hz tuning is approximately 261.63 Hz.

---

**👤 You:**
> "What are the first few harmonics of 100Hz?"

**🤖 AI Agent:**
> The harmonic series for 100Hz includes 200Hz, 300Hz, 400Hz, 500Hz, 600Hz, 700Hz, and 800Hz.


## Installation & Usage

To install and use the **Frequency & Note Converter** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/frequency-note-converter](https://vinkius.com/mcp/frequency-note-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
