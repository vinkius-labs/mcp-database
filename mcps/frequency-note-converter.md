# Frequency & Note Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/frequency-note-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Convert between musical frequencies and notes with precision.

## Description
A high-precision utility for musicians and audio engineers to bridge the gap between Hertz (Hz) and musical pitch. This MCP server provides tools like `frequency_to_note` to identify notes from frequencies, `note_to_frequency` for exact frequency calculation, `calculate_harmonics` for harmonic series generation, and `get_pitch_depth` to measure distance from the A0 baseline. Supports both 440Hz and 432Hz tuning standards.


## Available Tools (4)
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


## ❓ FAQ

**Q: What tuning standards are supported?**
The server supports the international standard (A4 = 440Hz) and the alternative tuning (A4 = 432Hz).

**Q: Can I calculate harmonics for any frequency?**
Yes, using the `calculate_harmonics` tool, you can generate the first 8 harmonics for any positive frequency.

**Q: How accurate are the conversions?**
The server provides precise semitone and cents deviation calculations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/frequency-note-converter](https://vinkius.com/mcp/frequency-note-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Frequency & Note Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `frequency-note-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Frequency & Note Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "frequency-note-converter": {
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
