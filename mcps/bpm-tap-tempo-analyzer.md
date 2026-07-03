# BPM Tap Tempo Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bpm-tap-tempo-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [music](../categories/music.md)

Analyze tap-based rhythmic input to derive precise tempo, stability, and musical context.

## Description
The BPM Tap Tempo Analyzer is a specialized engine for processing raw rhythmic taps. By providing an array of millisecond timestamps, you can use tools like `compute_tap_metrics` to calculate precise beats per minute (BPM) using weighted averaging and outlier detection. The server also provides `generate_musical_suggestions` to find half-time and double-time alternatives, and `audit_tap_integrity` to quantify the reliability of your tapping session based on interval consistency.


## Available Tools (3)
- **audit_tap_integrity**: Quantifies the quality and reliability of the tap sequence
- **compute_tap_metrics**: Processes raw tap data to determine the primary tempo and consistency metrics
- **generate_musical_suggestions**: Translates a raw BPM into musically useful rhythmic alternatives


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BPM Tap Tempo Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the BPM for these taps: [1000, 2000, 3000, 4000]"

**🤖 AI Agent:**
> The calculated BPM is 60.0 with a stability score of 0.0%.

---

**👤 You:**
> "What are the musical suggestions for 120 BPM?"

**🤖 AI Agent:**
> For 120 BPM, the rounded tempo is 120, the half-time suggestion is 60, and the double-time suggestion is 240.

---

**👤 You:**
> "Check if this tap sequence is reliable: [1000, 2100, 3050, 4200]"

**🤖 AI Agent:**
> The audit shows 0 outliers. The session is marked as reliable.


## ❓ FAQ

**Q: How do I use the `compute_tap_metrics` tool?**
Provide an array of millisecond timestamps representing each tap. The tool will filter out outliers and return the calculated BPM, stability score, and effective tap count.

**Q: What does the stability score represent?**
The stability score measures how much your tapping intervals fluctuate relative to the mean. A lower percentage indicates a more consistent and steady rhythm.

**Q: Can I get rhythmic alternatives for my tempo?**
Yes, by using the `generate_musical_suggestions` tool with a base BPM, you can automatically receive rounded, half-time, and double-time tempo values.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bpm-tap-tempo-analyzer](https://vinkius.com/mcp/bpm-tap-tempo-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BPM Tap Tempo Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bpm-tap-tempo-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BPM Tap Tempo Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bpm-tap-tempo-analyzer": {
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
