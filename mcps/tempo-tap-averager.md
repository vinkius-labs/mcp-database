# Tempo Tap Averager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tempo-tap-averager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [music](../categories/music.md)

Calculate precise BPM and rhythmic stability from tap timestamps.

## Description
The Tempo Tap Averager MCP server allows you to derive accurate musical tempo (BPM) and rhythm consistency from a sequence of millisecond timestamps. By using tools like `calculate_bpm` for precise BPM calculation, `evaluate_rhythm_consistency` for stability analysis, and `get_tempo_metadata` for musical descriptors, you can transform raw tap data into professional rhythmic insights.


## Available Tools (3)
- **calculate_bpm**: g., [0, 500, 1000]). Returns exact BPM, standard BPM, and suggested half/double time tempos.

Calculate BPM and tempo variations from tap timestamps
- **evaluate_rhythm_consistency**: Returns a stability score (0-1) and the number of detected outliers.

Evaluate the stability and consistency of a tapped rhythm
- **get_tempo_metadata**: g., 120). Returns the corresponding musical term (e.g., Vivace).

Get the musical label for a specific BPM


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tempo Tap Averager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the BPM for these taps: [0, 500, 1000, 1500, 2000]"

**🤖 AI Agent:**
> The calculated BPM is 120.0. Suggested tempos: 60 BPM (half-time) and 240 BPM (double-time).

---

**👤 You:**
> "How steady is this rhythm: [0, 480, 970, 1450, 1930]"

**🤖 AI Agent:**
> The stability score is 0.95 with 0 outliers detected.

---

**👤 You:**
> "What is the musical term for 140 BPM?"

**🤖 AI Agent:**
> The musical label for 140 BPM is Allegro.


## ❓ FAQ

**Q: How do I provide the input data?**
You should provide an array of numbers representing timestamps in milliseconds. For example, `[0, 500, 1000, 1500]`.

**Q: What does the stability score mean?**
The stability score is a value between 0 and 1. A score of 1 indicates perfectly consistent intervals, while lower scores indicate irregular tapping.

**Q: Can I get musical terms for my BPM?**
Yes, using the `get_tempo_metadata` tool, you can retrieve standard musical labels like 'Allegro' or 'Adagio' based on your calculated BPM.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tempo-tap-averager](https://vinkius.com/mcp/tempo-tap-averager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tempo Tap Averager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tempo-tap-averager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tempo Tap Averager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tempo-tap-averager": {
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
