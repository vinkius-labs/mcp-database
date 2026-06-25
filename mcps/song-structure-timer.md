# Song Structure Timer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/song-structure-timer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate musical timing, section durations, and full song timelines based on BPM and meter.

## Description
The Song Structure Timer is a precision utility for musicians and producers to calculate the exact timing of musical segments. By providing the BPM (Beats Per Minute) and time signature, you can use `get_bar_rhythm_metrics` to find the duration of beats and bars. The tool also allows you to calculate specific section lengths with `calculate_section_duration` and generate a complete, timestamped song timeline using `generate_song .song_timeline`. This is essential for recording reference, arrangement planning, and mastering.


## Available Tools (3)
- **get_bar_rhythm_metrics**: Calculate seconds per beat and seconds per bar
- **calculate_section_duration**: Calculate the length of a song section
- **generate_song_timeline**: Generate a complete structural breakdown of a song


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Song Structure Timer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the duration of one beat at 120 BPM in 4/4 time?"

**🤖 AI Agent:**
> At 120 BPM, a single beat lasts exactly 0.5 seconds.

---

**👤 You:**
> "Calculate the duration of a 16-bar verse if one bar is 2 seconds long."

**🤖 AI Agent:**
> A 16-bar verse with a 2-second bar duration will last 32 seconds.

---

**👤 You:**
> "Generate a timeline for a song at 100 BPM, 4/4 time, with an Intro of 8 bars and a Chorus of 16 bars."

**🤖 AI Agent:**
> The timeline starts with the Intro at 0:00 (lasting 16 seconds), followed by the Chorus starting at 0:16 (lasting 32 seconds).


## ❓ FAQ

**Q: How do I calculate the duration of a single beat?**
Use the `get_bar_ rhythm_metrics` tool. By inputting your current BPM and the number of beats per bar, it will return the exact duration in seconds for both a single beat and a full bar.

**Q: Can I generate a timeline for an entire song?**
Yes, the `generate_song_timeline` tool allows you to input your BPM, meter, and a list of sections (like Intro, Verse, Chorus) with their respective bar counts to produce a complete timestamped breakdown.

**Q: How is the section duration calculated?**
The `calculate_section_duration` tool takes the number of bars in a section and the duration of one bar (obtained from rhythm metrics) to calculate the total time in seconds, minutes, and a formatted MM:SS string.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/song-structure-timer](https://vinkius.com/mcp/song-structure-timer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Song Structure Timer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `song-structure-timer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Song Structure Timer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "song-structure-timer": {
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
