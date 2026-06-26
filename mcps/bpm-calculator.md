# BPM Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bpm-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Convert BPM into rhythmic durations, frequencies, and musical tempo classifications.

## Description
The BPM Calculator is a precision utility for musicians. It allows you to convert beats per minute (BPM) into exact rhythmic durations in milliseconds and frequencies in Hertz. Using tools like `calculate_all_durations`, you can get a complete breakdown of note values including whole, half, quarter, eighth, sixteenth, and thirty-second notes, as well as their dotted and triplet versions. You can also use `get_tempo_classification` to translate numerical BPM into historical musical terms like Adagio or Allegro, and `list_supported_subdivisions` to see all available rhythmic patterns.


## Available Tools (3)
- **get_tempo_classification**: g., "Moderato").

Translates a numerical BPM value into its descriptive musical terminology
- **list_supported_subdivisions**: Returns a registry of all note types supported by the calculator
- **calculate_all_durations**: Provides a complete breakdown of all supported note durations and their corresponding frequencies for a specific BPM


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BPM Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the durations and frequencies for 120 BPM?"

**🤖 AI Agent:**
> At 120 BPM, a quarter note lasts 500 ms with a frequency of 2 Hz. A whole note lasts 2000 ms at 0.5 Hz.

---

**👤 You:**
> "Classify a tempo of 80 BPM."

**🤖 AI Agent:**
> A tempo of 80 BPM is classified as Andante.

---

**👤 You:**
> "List all the note subdivisions you can calculate."

**🤖 AI Agent:**
> The supported subdivisions include Whole Note, Half Note, Quarter Note, Eighth Note, Sixteenth Note, and Thirty-second Note, along with their dotted and triplet variations.


## ❓ FAQ

**Q: How can I see the duration of a quarter note in milliseconds?**
Use the `calculate_all_durations` tool with your current BPM. It will return the duration in ms for all supported notes, including the quarter note.

**Q: What does 'Adagio' mean in terms of BPM?**
You can use the `get_tempo_classification` tool to find the specific BPM range for Adagio or any other musical tempo marking.

**Q: Does this calculator support triplet notes?**
Yes, the `calculate_all_durations` tool includes calculations for triplet versions of supported note values.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bpm-calculator](https://vinkius.com/mcp/bpm-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BPM Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bpm-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BPM Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bpm-calculator": {
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
