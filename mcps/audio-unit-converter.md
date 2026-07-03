# Audio Unit Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/audio-unit-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Convert between musical frequencies, rhythmic durations, digital sample counts, and logarithmic amplitude levels.

## Description
The Audio Unit Converter provides precise mathematical conversions for audio engineering and music production. Use `convert_pitch_identity` to translate between Hertz, note names, and MIDI numbers with cents deviation. Utilize `convert_sample_timing` to calculate the relationship between milliseconds and sample counts at any given sample rate. The `calculate_tempo_rhythm` tool allows you to determine the exact duration of musical subdivisions like eighth or sixteenth notes based on BPM. Finally, `convert_amplitude_magnitude` handles the conversion between logarithmic decibel levels (dBFS, dBu, dBV) and linear amplitude ratios.


## Available Tools (4)
- **convert_amplitude_magnitude**: Convert between decibels and linear amplitude
- **convert_pitch_identity**: Convert between frequency, note name, and MIDI number
- **calculate_tempo_rhythm**: Calculate rhythmic subdivision durations based on BPM
- **convert_sample_timing**: Convert between duration in ms and sample count


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Audio Unit Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the frequency of note A4 if the tuning is 440Hz?"

**🤖 AI Agent:**
> The frequency for A4 at a 440Hz tuning reference is exactly 440.0 Hz.

---

**👤 You:**
> "How many samples are in 500ms at a 44100Hz sample rate?"

**🤖 AI Agent:**
> At a sample rate of 44100Hz, 500 milliseconds corresponds to 22,050 samples.

---

**👤 You:**
> "What is the duration of an eighth note at 120 BPM?"

**🤖 AI Agent:**
> At 120 BPM, an eighth note lasts 250.0 milliseconds.


## ❓ FAQ

**Q: How accurate are the frequency conversions?**
The `convert_pitch_identity` tool provides highly precise calculations, including cents deviation from standard tuning references like 440Hz or 432Hz.

**Q: Can I convert between milliseconds and samples?**
Yes, using `convert_sample_timing`, you can translate durations in milliseconds to sample counts (and vice versa) as long as you provide the sample rate.

**Q: Does it support different decibel scales?**
Yes, `convert_amplitude_magnitude` supports conversions for dBFS, dBu, and dBV scales.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/audio-unit-converter](https://vinkius.com/mcp/audio-unit-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Audio Unit Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `audio-unit-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Audio Unit Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "audio-unit-converter": {
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
