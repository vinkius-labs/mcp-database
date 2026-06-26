# Interval Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/interval-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Calculate musical intervals, properties, and note frequencies.

## Description
An essential tool for musicians and theorists to calculate the distance between notes in semitones, identify interval qualities (such as Major 3rd or Perfect 5th), determine stability (consonant vs. dissonant), and compute precise frequencies in Hz using A4=440Hz or A4=432Hz tuning standards. Use `calculate_semitone_distance` for raw distance, `identify_interval_properties` for musical character, and `calculate_note_frequency` for frequency calculations.


## Available Tools (3)
- **identify_interval_properties**: Describe the musical character and identity of an interval
- **calculate_note_frequency**: Determine the physical vibration frequency for a specific note
- **calculate_semitone_distance**: g., "C4") and end note (e.g., "E4") and returns total semitones moved.

Find the raw numerical distance between two pitches in semitones


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Interval Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the distance in semitones between C4 and G4?"

**🤖 AI Agent:**
> The distance between C4 and G4 is 7 semitones.

---

**👤 You:**
> "Tell me about the interval between D4 and F4."

**🤖 AI Agent:**
> The interval from D4 to F4 is a Minor 3rd, which is classified as Dissonant. Its inversion is an Augmented 6th.

---

**👤 You:**
> "What is the frequency of A4 using 432Hz tuning?"

**🤖 AI Agent:**
> The frequency of A4 with a 432Hz tuning standard is 432.0 Hz.


## ❓ FAQ

**Q: How do I find the distance between two notes?**
Use the `calculate_semitone_distance` tool by providing the starting note and the ending note (e.g., 'C4' and 'E4'). It will return the total number of semitones between them.

**Q: Can I check if an interval is consonant or dissonant?**
Yes, use the `identify_interval_properties` tool. It will tell you if the interval is classified as 'Consonant' or 'Dissonant', along with its name and inversion.

**Q: How do I calculate the frequency of a specific note?**
Use the `calculate_note_frequency` tool. You need to provide the note name, the octave, and choose between '440Hz' or '432Hz' as your tuning standard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/interval-calculator](https://vinkius.com/mcp/interval-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Interval Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `interval-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Interval Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "interval-calculator": {
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
